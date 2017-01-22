## Week 5 Outline: Web Scraping & APIs


### Class Objectives
- Download individual files, file lists, and entire websites using wget.
- Scrape structured data from Wikipedia.
- Access JSON data via APIs and re-formatting in tabular form.

#### Wget intro
We used Wget briefly in our first class, but today we’ll try out a few more advanced features. As we saw then, downloading the HTML source for a particular page is as easy as passing its url to Wget.

	wget http://example.com

 If we want to download a series of files, we can list their URLs in a text document and download them all using the `--input` or `-i` option. You can assemble a list yourself or try it out with [this](https://www.dropbox.com/s/e8quww6kixusflw/Ten_URLs.txt?dl=1) set of 10 random Wikipedia URLs.

	wget -i Ten_URLs.txt

Wget also supports recursive downloading. Download an entire website like so:

	wget ‐‐execute robots=off ‐‐recursive ‐‐no-parent ‐‐continue ‐‐no-clobber http://example.com/

You can also download a series of sequentially numbered files with following notation:

	wget http://example.com/images/{1..20}.jpg
	wget https://www.discogs.com/release/84319{10..25}


#### Beautiful Soup basics


#### In-Class Exercise: Scraping a Metadata Set from Wikipedia
- Choose a list of related Wikipedia articles (e.g., [The Top 100 Crime Novels of All Time](https://en.wikipedia.org/wiki/The_Top_100_Crime_Novels_of_All_Time)). 
  - More options: [List of lists of lists](https://en.wikipedia.org/wiki/List_of_lists_of_lists#Literature)
- Download the list using Beautiful Soup and create a list of URLs for each page.
- Download each page on the list and extract relevant metadata (author, language, genre, publisher, date, page count, etc.).
- Export data as a CSV.

- Sample code for Wikipedia list scraping: [http://chrisalbon.com/python/beautiful\_soup\_scraping\_into\_pandas.html](http://chrisalbon.com/python/beautiful_soup_scraping_into_pandas.html)



#### ElementTree XML parser in Python

	import xml.etree.ElementTree as ET
	tree = ET.parse('/Users/yourname/Desktop/sandbox/country_data.xml')
	root = tree.getroot()
	
	for child in root:
		print child.tag, child.attrib

#### Discuss HTML, XML, and HTML5

#### Working with API Data
CrossRef metadata search:
- http://search.crossref.org/help/api
- http://search.crossref.org/dois?q=renear+palmer&sort=score
- http://search.crossref.org/dois?q=10.5555%2F12345678

#### Exercise
Download a dataset of choice via API, convert to CSV, and clean using OpenRefine or Excel.