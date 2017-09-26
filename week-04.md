## Week 4: Collections as Data: Data Models

Launch your Docker Container and open a new Jupyter Notebook.

#### Working with JSON
JSON data is a representation of key-value pairs, very much like a dictionary in Python. For the following example we’ll download a JSON version of the artwork metadata we’ve been working with.

```python3
import urllib2
url="https://github.com/MuseumofModernArt/collection/blob/master/Artworks.json?raw=true"
json_string=urllib2.urlopen(url).read()
json_data = json.loads(json_string)
```
To view JSON data (as well as dictionaries and just about any other data format), Python offers a “pretty printer” module. There are also numerous online tools for prettifying JSON data, such as [these](http://jsonviewer.stack.hu/) [two](http://json.parser.online.fr/beta/).

```python3
from pprint import pprint
pprint(json_data)
```

To examine the top-level keys in our JSON data, enter the following.

```python3
for key in json_data:
    print(key)
```

> *Output*:
>
>     records
>     meta

In this case, the “records” key points to a list of item records. The following will return the first record.

```python3
print(json_data['records'][0])
```

> *Output:*
>
>     \{u'pk': 19579, u'model': u'collection.museumobject', u'fields': \{u'primary_image_id': u'2006AJ6728', u'object': u'Cabinet', u'year_start': 1600, u'artist': u'Fiamengo, Iacopo', u'museum_number': u'W.36:1, 2-1981', u'rights': 3, u'object_number': u'O61539', u'last_processed': u'2016-04-30 02:11:57', u'event_text': u'', u'collection_code': u'FWK', u'place': u'Naples', u'longitude': u'14.25185000', u'last_checked': u'2016-04-30 02:11:57', u'museum_number_token': u'w361981', u'latitude': u'40.83990100', u'title': u'', u'date_text': u'about 1600 (Made)\nca. 1600 (made)', u'slug': u'cabinet-fiamengo-iacopo', u'sys_updated': u'2015-12-11 00:00:00', u'location': u'Europe 1600-1815, room 6, case CA11'\}\}


A record, in turn, contains three keys: “pk,” “model,” and “fields.”

```python3
print(json_data['records'][0])
```

> *Output:*
>
>     pk
>     model
>     fields

The metadata we’re interested in is under “fields.”

```python3
for key in json_data['records'][0]['fields']:
    print(key)
```

> *Output:*
>
>     primary_image_id
>     object
>     year_start
>     artist
>     museum_number
>     rights
>     object_number
>     last_processed
>     event_text
>     collection_code
>     place
>     longitude
>     last_checked
>     museum_number_token
>     latitude
>     title
>     date_text
>     slug
>     sys_updated
>     location

We can thus view the “artist” field like so.

```python3
print(json_data['records'][0]['fields']['artist'])
```

#### JSON Data to CSV
Next we’ll transfer these metadata fields to CSV format. First, let’s create a list of column titles for reference:

```python3
header=[]

for key in json_data['records'][0]['fields']:
    header.append(key)

print(header)
```
Then we’ll use our column titles (which are also keys in the “fields” key-value set) to create a list of rows for our CSV. Since the CSV writer prefers working with non-Unicode strings, we’ll use the `str()` function to reformat each metadata item as we add it to the table.

```python3
meta_table=[]

for record in json_data['records']:
    row=[]
    for key in header:
        row.append(unidecode(record['fields'][key]))
    meta_table.append(row)

print(meta_table[0])
```

Now let’s make a string version of our header.

```python3
header_string=[]

for item in header:
    header_string.append(str(item))
```
Finally, we’ll write our metadata collection as a CSV.

```python3
import csv
outpath="/sharedfolder/V_and_A_ivory.csv"
o = open(outpath, 'w')
a = csv.writer(o)
a.writerows([header_string])
a.writerows(meta_table)
o.close()
```
Open your CSV in Excel or Calc.


#### OpenRefine

Open a new terminal window and runt the following command to download and run a Dockerized copy of the tabluar data cleaning program OpenRefine.

```
docker run --name openrefine -d -p 3334:3333 psychemedia/docker-openrefine
```

Enter the following address in your browser’s URL bar to open the application.

- [http://127.0.0.1:3334/](http://127.0.0.1:3334/)

Click `Create Project`, then `Choose Files` and choose `V_and_A_ivory.csv`. Click `Next`. In the following window, click `Create Project` in the upper right corner.

At the top of the “place” column, click the dropdown button and choose “Text Facet.” A list of places will appear in the left column. Click “Paris” to display only works created there.

Note that several “place” records are listed as “Germany,” while others are German cities. Let’s group them under a single facet.
