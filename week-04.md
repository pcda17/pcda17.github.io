## Week 4: Collections as Data: Data Models

Launch your Docker Container and open a new Jupyter Notebook.

#### Working with JSON
JSON data is a representation of key-value pairs, very much like a dictionary in Python. For the following example we’ll download a JSON version of the artwork metadata we’ve been working with.

```python3
import json
from urllib.request import urlopen

url = "https://media.githubusercontent.com/media/MuseumofModernArt/collection/master/Artworks.json?raw=true"
json_string = urlopen(url).read().decode('utf8')
json_data = json.loads(json_string)
```
To view JSON data (as well as dictionaries and just about any other data format), Python offers a “pretty printer” module. Here we are viewing the first 200 artworks in the metadata set.

There are also numerous online tools for prettifying JSON data, such as [these](http://jsonviewer.stack.hu/) [two](http://json.parser.online.fr/beta/).

```python3
from pprint import pprint

pprint(json_data[:200])
```

Much like a dictionary object in Python, a JSON object is made up of key-value pairs that can contain (and be contained in) lists. In this case, MoMA has presented metadata for its artworks as a list of key-value pairs.

To see the number of artworks included in the JSON object, use the `len()` function.

```
len(json_data)
```

To view the key-value metadata for a random artwork, use `random.choice()`.

```
import random

random.choice(json_data)
```

Using bracket notation, we can access individual metadata fields by their keys. Here we display several metadata fields for a randomly chosen artwork.

```
artwork = random.choice(json_data)

print(artwork['Artist'])
print(artwork['Title'])
print(artwork['Date'])
print(artwork['AccessionNumber'])
print(artwork['URL'])
```

The following loop will print the `Artist` field for the first 100 artworks in the list.

```python3
for item in json_data[:100]:
    pprint(item['Artist'])
```

You can also use `random.sample()` to view artist names for 100 artworks chosen at random.

```
for item in random.sample(json_data, 100):
    pprint(item['Artist'])
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
out_path="/sharedfolder/V_and_A_ivory.csv"

with open(out_path, 'w') as fo:
    csv_out = csv.writer(fo)
    csv_out.writerows([header_string])
    csv_out.writerows(meta_table)
```
Open your CSV in Excel or Calc.


#### OpenRefine

OpenRefine is very easy to download and run from your computer. You can get the download here: [http://openrefine.org/](http://openrefine.org/).

Open a new terminal window and run the following command to download and run a Dockerized copy of the tabluar data cleaning program OpenRefine.

```
docker run --name openrefine -d -p 3334:3333 psychemedia/docker-openrefine
```

Enter the following address in your browser’s URL bar to open the application.

- [http://127.0.0.1:3334/](http://127.0.0.1:3334/)

Today's OpenRefine tutorial is in this week's files on Canvas.

<!--
Click `Create Project`, then `Choose Files` and choose `V_and_A_ivory.csv`. Click `Next`. In the following window, click `Create Project` in the upper right corner.

At the top of the “place” column, click the dropdown button and choose “Text Facet.” A list of places will appear in the left column. Click “Paris” to display only works created there.

Note that several “place” records are listed as “Germany,” while others are German cities. Let’s group them under a single facet.
-->
