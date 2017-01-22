Syllabus: Programming for Cultural Data Analysis
====================================================

Designed by Stephen McLaughlin with Tanya Clement

University of Texas at Austin School of Information

2016–17


### Course Objectives

-   Teach scripting-style programming in Python and Unix-like systems, emphasizing literacy in finding and using free and open source software.

-   Familiarize students with techniques for collecting, transforming, and analyzing media and metadata available on the Web.

-   Introduce commonly used data models and their standard formats, including CSV, JSON, and XML.

-   Explore computational text analysis techniques such as natural language processing (NLP), sentiment analysis, and machine learning classification.

-   Introduce tools for analyzing cultural data via visualization and statistical tests, emphasizing critical reflection on the limitations of these approaches.

-   Familiarize students with Web archiving and data curation practices.

-   Explore cultural implications of large-scale preservation of cultural materials.


### Course Principles

-   Imitating and modifying others’ code is essential in learning to program. You can many examples and explanations on [Stack Exchange](http://stackexchange.com) and similar online forums. Taking one or two lines without attribution is OK; if you use a longer chunk of code found online, add a #comment with the source’s URL.

-   Begin assignments early. If you realize what you had in mind is more difficult than expected, talk to the instructor about choosing an alternative.

-   We’ll be focusing on a scripting approach to programming. This course is not oriented toward developing large, complex programs or writing perfectly optimized code.

-   Learning to code takes trial and error. Work through weekly programming tutorials before class and continue polishing in-class coding assignments at home.

### Final Project: Critical Data Analysis

For your final project, you will construct a dataset drawn from two or more online sources and analyze those data in a critical essay. You may either present an argument about the data (e.g., describing bias in the way the data were chosen and arranged by a cultural institution) or you may use your dataset as the basis for an argument about culture (e.g., tracing a stylistic shift in a literary community). You should conceive and execute your project with a specific audience in mind, such as literary scholars, newspaper readers, or policy advocates.

Your dataset should comprise at least 200 texts or other media files, or at least 1000 metadata records. The size of your collection should be appropriate to your technical skills and the complexity of each record. Rather than using a pre-existing dataset, you should extend the collection in some way. This might mean curating material from multiple sources, mashing up two or more datasets, augmenting records using machine learning or natural language processing, or using a creative technique to organize messy data.

Your final project will include the following elements:

-   Extended dataset (submitted week 9 in draft form)

-   In-class presentation (week 14)

-   4–5-page critical essay, including 3–4 data visualizations

-   1-page description of your chosen research genre and intended audience, as well as a reflection on the strengths and weaknesses of your method

-   Jupyter notebook containing code used for data analysis and visualization

### Weekly Assignments

Assignments should be posted on Canvas before the start of class each week.

### Resources

-   Software Tools

-   Sample Data Sources



Week 1: Introductions & Command Line Basics
===========================================


To Do Before Class
------------------

To access Lynda videos, follow links below, click “Log in,” then “Organizational Login,” and enter your UT EID and password.

- Optional: Allardice, Simon. “Foundations of Programming: Fundamentals.” Lynda.com. [http://www.lynda.com/JavaScript-tutorials/Foundations-of-Programming-Fundamentals/83603-2.html](http://www.lynda.com/JavaScript-tutorials/Foundations-of-Programming-Fundamentals/83603-2.html)

- Optional: Marini, Joe. “Up and Running with Python.” Lynda.com.
            [http://www.lynda.com/Python-tutorials/Welcome/122467/142550-4.html](http://www.lynda.com/Python-tutorials/Welcome/122467/142550-4.html)

Laptop users only:

-   Update Max OS X to its latest version.

-   Install the following programs:

    -   [TextWrangler](http://www.barebones.com/products/textwrangler/) (plain text editor)

    -   [VLC Media Player](http://www.videolan.org/vlc/index.html)

If you don’t have Excel, you should install the [OpenOffice](http://www.openoffice.org/download) suite, which includes a spreadsheet program called Calc. We won’t need it for today’s class.

Note that the university caps each student’s wi-fi bandwidth use at 1 GB per week. During class, laptop users should use an Ethernet connection and/or [purchase additional wi-fi bandwidth](https://www.utexas.edu/its/help/network/403).

##### ▸ In-Class Outline




Week 2: Python Intro and Text Manipulation
==========================================


To Do Before Class
------------------

Read pages 1–28 of Shieber’s Python tutorial and work through the code examples.

Work through Chris Albon’s tutorial on Python string operations.


Reading
-------

-   Shieber, Stuart M., *Programming for Humanists* pages 1–28, 2014. [http://blogs.harvard.edu/programmingforhumanists/files/2014/12/proghum.pdf](http://blogs.harvard.edu/programmingforhumanists/files/2014/12/proghum.pdf)

-   Montfort, Nick. “Why Program?” In *Exploratory Programming for the Arts and Humanities*, 267–77. Cambridge, MA: The MIT Press, 2016. [PDF](https://www.dropbox.com/s/kb2xy8giavxpo89/Montfort%202016%20-%20Why%20Program.pdf?dl=0).

-   Albon, Chris. “String Operations.” [http://chrisalbon.com/python/string_operations.html](http://chrisalbon.com/python/string_operations.html)

-   Oualline, Steve. “The End of Line Puzzle.” *The Practical Programmer*. [http://www.oualline.com/practical.programmer/eol.html](http://www.oualline.com/practical.programmer/eol.html)



Optional Reading
----------------

-   Noria, Xavier. “Understanding Newlines.” *O’Reilly ONLamp*, August 17, 2006. [http://www.onlamp.com/pub/a/onlamp/2006/08/17/understanding-newlines.html](http://www.onlamp.com/pub/a/onlamp/2006/08/17/understanding-newlines.html)

-   Stephenson, Neal. “In the Beginning Was the Command Line.” Cryptonomicon, 1999. <http://www.cryptonomicon.com/beginning.html>. [TXT](http://www.cryptonomicon.com/command.zip). [PDF](https://www.dropbox.com/s/kbpvllkmlb7u5uh/Neal%20Stephenson%201999%20-%20In%20the%20Beginning%20was%20the%20Command%20Line.pdf?dl=1). [EPUB](https://www.dropbox.com/s/sisnsmw0m0b6vci/Neal%20Stephenson%201999%20-%20In%20the%20Beginning%20was%20the%20Command%20Line.epub?dl=0).

##### ▸ In-Class Outline


Week 3: Data Models
===================

> Note: In this course we will primarily work with data in CSV and JSON formats. Relational databases and RDF are discussed in readings but will not be emphasized in class.


To Do Before Class
------------------

Choose an online data/metadata source, preferably one available to the public via direct download or API. Download a sample of the data, at least 50 or 100 records. Read them over closely, noting anything unexpected. Search for information about the dataset's history, purpose, intended audience, and any past uses by researchers or journalists. Describe what you learned in 400–500 words.

Create a Jupyter notebook document and familiarize yourself with the interface.

Install [OpenRefine](https://github.com/OpenRefine/OpenRefine/wiki/Installation-Instructions) and create a project using a sample dataset. Familiarize yourself with some of its basic functions.

> • Like Jupyter, OpenRefine creates a locally accessible “server” and uses a browser window for its interface. If launching OpenRefine doesn’t open a browser window automatically, enter the following in the URL bar: *http://127.0.0.1:3333*
>
> • If you’re working with very large datasets, you may need to allocate more memory for OpenRefine:
> [https://github.com/OpenRefine/OpenRefine/wiki/FAQ:-Allocate-More-Memory](https://github.com/OpenRefine/OpenRefine/wiki/FAQ:-Allocate-More-Memory)


Readings
--------

-   van Hooland, Seth, and Ruben Verborgh. “Modelling.” In *Linked Data for Libraries, Archives and Museums: How to Clean, Link and Publish Your Metadata*, 11–70. Chicago: Neal-Schuman, 2014. [PDF](https://www.dropbox.com/s/uv9xhmiq574rbyj/van%20Hooland%20and%20Verborgh%202014%20-%20Modelling.pdf?dl=0).

-   Swartz, Aaron. “Building a Platform: Providing APIs.” In *Aaron Swartz’s ‘A Programmable Web’: An Unfinished Work*, 31–39. San Rafael, CA: Morgan & Claypool Publishers, 2013. [PDF](https://www.dropbox.com/s/wmgtcko0u9q59aw/Swartz%202013%20-%20Building%20a%20Platform-%20Providing%20APIs.pdf?dl=0).

-   Posner, Miriam. “Humanities Data: A Necessary Contradiction.” *Miriam Posner’s Blog*, June 25, 2015. *http://miriamposner.com/blog/humanities-data-a-necessary-contradiction*

-   “The Jupyter Notebook.” [http://jupyter-notebook.readthedocs.io/en/latest/notebook.html](http://jupyter-notebook.readthedocs.io/en/latest/notebook.html)

-   Albon, Chris. “Parse JSON File.” [http://chrisalbon.com/python/json_parse_file.html](http://chrisalbon.com/python/json_parse_file.html)



Optional Readings
-----------------

-   Fortune, Stephen. “A Brief History of Databases.” *Avant*, February 27th 2014. [https://web.archive.org/web/20150220031213/http://avant.org/media/history-of-databases](https://web.archive.org/web/20150220031213/http://avant.org/media/history-of-databases)

-   Lundh, Fredrik. “Elements and Element Trees.” [http://effbot.org/zone/element.htm](http://effbot.org/zone/element.htm) [Python XML tutorial]

-   Beazley, David, and Brian K. Jones. “Chapter 6: Data Encoding and Processing.” In Python Cookbook: *recipes for Mastering Python 3*, 3. ed., 175–216. Bejing: O’Reilly, 2013. [PDF](https://www.dropbox.com/s/750hh3tych80v68/Python_Cookbook_3rd-ed_Ch-6.pdf?dl=0)

-   Zhuang, Atima Han, Ishita Vedvyas, and Rishikesh Dole. “Tutorial: OpenRefine,” 2013. [http://casci.umd.edu/wp-content/uploads/2013/12/OpenRefine-tutorial-v1.5.pdf](http://casci.umd.edu/wp-content/uploads/2013/12/OpenRefine-tutorial-v1.5.pdf)

-   Introna, L. D. “The Enframing of Code: Agency, Originality and the Plagiarist.” *Theory, Culture & Society* 28, no. 6 (November 1, 2011): 113–41. [PDF](https://www.dropbox.com/s/s0zmg1iw308vb4e/Introna%202011%20-%20The%20Enframing%20of%20Code-%20Agency%2C%20Originality%20and%20the%20Plagiarist.pdf?dl=0).

##### ▸ In-Class Outline


Week 4: Word-Level Text Analysis
================================


To Do Before Class
------------------

Install textblob package before class (a wrapper for NLTK and pattern) and work through Montfort’s code examples. The --user option lets us install a module for the current user only, without requiring an admin password.

> pip install --user -U textblob
>
> python -m textblob.download_corpora

Choose a book-length text (or set of texts) available online with which you are familiar. Following Montfort’s code examples, parse the text using the TextBlob library and run some exploratory tests. In 400–500 words, describe your process and what you learned about the text, emphasizing anything you found surprising. Submit your code in a Jupyter notebook.


Readings
--------

-   Ramsay, Stephen. “Chapter 1: An Algorithmic Criticism.” In *Reading Machines: Toward an Algorithmic Criticism*, 1–17. Topics in the Digital Humanities. Urbana: University of Illinois Press, 2011. [PDF](https://www.dropbox.com/s/ox35us0vfj7ppng/Ramsay%202011%20-%20Reading%20Machines%20-%20Ch.%201.pdf?dl=0).

-   Montfort, Nick. “Text III.” In *Exploratory Programming for the Arts and Humanities*, 185–213. Cambridge, MA: The MIT Press, 2016. [PDF](https://www.dropbox.com/s/gib77npezdaz1kr/Montfort%202016%20-%20Text%20III.pdf?dl=0).

-   Fellenbaum, Christiane. “Wordnet(s).” In The *Encyclopedia of Language & Linguistics*, edited by E. K. Brown and Anne Anderson, 2nd ed., 14:665–79. Amsterdam ; Boston: Elsevier, 2005. [PDF](https://www.dropbox.com/s/zxuvhzlheiyo7uc/Fellenbaum%202005%20-%20Wordnet%28s%29.pdf?dl=0).

-   “Alphabetical list of part-of-speech tags used in the Penn Treebank Project.” [https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html](https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html)



Topics to Cover
---------------

-   comparing word frequency between authors

-   part-of-speech (POS) tagging

-   POS frequency comparison

-   Naive Bayes text classification

-   sentiment analysis

-   using WordNet

##### ▸ In-Class Outline


Week 5: Web Scraping & APIs
=============================


To Do Before Class 
-------------------

Install [Beauitful Soup](https://www.crummy.com/software/BeautifulSoup/) library for parsing HTML.

> pip install -U --user beautifulsoup

Work through Chris Albon’s Beautiful Soup tutorial.

Choose an API from the list of examples or choose one that is relevant to your final project. An API with a URL-based interface is preferable. Sign up for a developer key if necessary, keeping in mind that it may take a day or two for your request to be processed. Read the documentation for the API and familiarize yourself with it by running a few sample queries. Then execute a larger query (or series of queries) within bounds you choose, aiming to collect at least 2,000–3,000 metadata records. Verify that your dataset is complete and intact. Transform the data to CSV format and conduct any necessary cleaning in Excel, Calc, or OpenRefine. Post 100–200 words on Canvas about your collection process and results.


Readings
--------

-   Pomerantz, Jeffrey. “The Future of Metadata.” In *Metadata*. The MIT Press Essential Knowledge Series. Cambridge, MA ; London, England: The MIT Press, 2015. [PDF](https://www.dropbox.com/s/hj3i12cinl3ublj/Pomerantz%202015%20-%20Ch.%208%20-%20The%20Future%20of%20Metadata.pdf?dl=0).

-   Kelly, Chelsea Emelie. “Beyond Digital: Open Collections & Cultural Institutions,” 2014. *https://artmuseumteaching.com/2014/11/06/beyond-digital-open-collections-cultural-institutions*

-   “HTML Introduction” and “HTML5 Introduction.” W3Schools.

    -   [http://www.w3schools.com/html/html_intro.asp](http://www.w3schools.com/html/html_intro.asp)

    -   [http://www.w3schools.com/html/html5_intro.asp](http://www.w3schools.com/html/html5_intro.asp)

-   Albon, Chris. “Beautiful Soup Basic HTML Scraping.” [http://chrisalbon.com/python/beautiful_soup_html_basics.html](http://chrisalbon.com/python/beautiful_soup_html_basics.html)



Optional Readings
-----------------

-   Sanger, David E., and Eric Schmitt. “Snowden Used Low-Cost Tool to Best N.S.A.” The New York Times. February 8, 2014. [http://www.nytimes.com/2014/02/09/us/snowden-used-low-cost-tool-to-best-nsa.html](http://www.nytimes.com/2014/02/09/us/snowden-used-low-cost-tool-to-best-nsa.html)

-   Kazil, Jacqueline, and Katharine Jarmul. “PDFs and Problem Solving in Python.” In *Data Wrangling with Python: Tips and Tools to Make Your Life Easier*, 91–126. O’Reilly, 2016. [PDF](https://www.dropbox.com/s/hfc8m731eiik0g8/Kazil%20and%20Jarmul%202016%20-%20PDFs%20and%20Problem%20Solving%20in%20Python.pdf?dl=0).

> ▸ In-Class Outline


Week 6: Data and Politics
=========================


To Do Before Class
------------------

In 500–600 words, evaluate the “moral dimension” of the dataset you collected last week. Take the [list of questions](https://thefrailestthing.com/2014/11/29/do-artifacts-have-ethics/) posed by Michael Sacasas as a starting point, describing any biases, exclusions, or individual interests reflected in the collection. What can't these data tell you? How might they be used or misused?


Readings
--------

-   Peters, Justin. *The Idealist: Aaron Swartz and the Rise of Free Culture on the Internet*, Chapters 7 and 8. New York: Scribner, 2016. [PDF](https://www.dropbox.com/s/fg195av2ayiwc31/Peters%202016%20-%20The%20Idealist%20-%20Chs.%206-7.pdf?dl=0).

-   Greenwald, Glenn. “Chapter 1: Contact.” In *No Place to Hide: Edward Snowden, the NSA, and the U.S. Surveillance State*, 2015. [PDF](https://www.dropbox.com/s/1evnc6xu6pbdin6/Greenwald%202014%20-%20No%20Place%20to%20Hide%20-%20Intro%20%26%20Chapter%201.pdf?dl=0).

-   Julia Angwin, Jeff Larson, Surya Mattu and Lauren Kirchner, ProPublica. “Machine Bias.” *ProPublica*. May 23, 2016. [https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)

-   Freelon, Deen Goodwin, Charlton D. McIlwain, and Meredith D. Clark. “Beyond the Hashtags: #Ferguson, #Blacklivesmatter, and the Online Struggle for Offline Justice,” 2016. [http://cmsimpact.org/wp-content/uploads/2016/03/beyond_the_hashtags_2016.pdf](http://cmsimpact.org/wp-content/uploads/2016/03/beyond_the_hashtags_2016.pdf)

-   Sacasas, Michael. “Do Artifacts Have Ethics?” *The Frailest Thing*, November 29, 2014. [http://thefrailestthing.com/2014/11/29/do-artifacts-have-ethics](http://thefrailestthing.com/2014/11/29/do-artifacts-have-ethics/)

-   American Civil Liberties Union. "First Amendment Lawsuit Brought on Behalf of Academic Researchers and Journalists Who Fear Prosecution Under the Computer Fraud and Abuse Act." [https://www.aclu.org/news/aclu-challenges-law-preventing-studies-big-data-discrimination](https://www.aclu.org/news/aclu-challenges-law-preventing-studies-big-data-discrimination)



Optional Readings
-----------------

-   Day, Ronald E. “Governing Expression: Social Big Data and Neoliberalism.” In *Indexing It All: The Subject in the Age of Documentation*, Information, and Data, 123–44. History and Foundations of Information Science. Cambridge, Massachusetts: The MIT Press, 2014. [PDF](https://www.dropbox.com/s/mab080ymg2pqjon/Day%202014%20-%20Indexing%20it%20All%20-%20Ch.%206%20-%20Governing%20Expression-%20Social%20Big%20Data%20and%20Neoliberalism.pdf?dl=0).

-   Hitchcock, Tim. “Digital Searching and the Re-formulation of Historical Knowledge” 2008. In *The Virtual Representation of the Past*, edited by Mark Greenglass and Lorna Hughes, 81-90. Ashgate: 2008. [PDF](https://www.dropbox.com/s/ht8si4vygm3bkh4/Hitchcock%202008%20-%20Digital%20Searching%20and%20the%20Re-formulation%20of%20Historical%20Knowledge.pdf?dl=0).

-   Winner, Langdon. “Do Artifacts Have Politics?” *Daedalus* 109, no. 1 (1980): 121–36. [PDF](https://www.dropbox.com/s/ttr620gqbv4tj48/Winner%201980%20-%20Do%20Artifacts%20Have%20Politics%3F.pdf?dl=0).

-   Joerges, B. “Do Politics Have Artefacts?” *Social Studies of Science* 29, no. 3 (June 1, 1999): 411–31. [PDF](https://www.dropbox.com/s/mb8cn5trvphm3oz/Joerges%201999%20-%20Do%20Politics%20Have%20Artefacts.pdf?dl=0).

##### ▸ In-Class Outline


Week 7: Statistics and Visualization
====================================


To Do Before Class
------------------

Submit a 500–700-word proposal for your final critical data analysis project. What data will you be using? What kind of patterns are you looking for? What critical lens will you apply? Most importantly, who is the intended audience for your study and why would/should they care about your findings? Describe what led you to choose this project and present any preliminary observations and hypotheses. You should consider this assignment an abstract or partial draft toward your final project.

Each student should post the proposal two days before class. You will be assigned another student at random, and you will post a 100–200-word response to that student’s proposal before class.

Install [numpy](http://www.numpy.org/) scientific computing library for Python.

> pip install --user -U numpy

Install [pandas](http://pandas.pydata.org/) data analysis library for Python.

> pip install --user -U pandas

Install [matplotlib](http://matplotlib.org/) visualization library for Python.

> pip install --user -U matplotlib


Readings
--------

-   Montfort, Nick. Excerpt from “Statistics and Visualization.” In *Exploratory Programming for the Arts and Humanities*, 215–40. Cambridge, MA: The MIT Press, 2016. [PDF](https://www.dropbox.com/s/7ihzxmrcq2997e4/Montfort%202016%20-%20Statistics%20and%20Visualization.pdf?dl=0).

-   Burrows, John. “Textual Analysis.” In *Companion to Digital Humanities*, edited by Susan Schreibman, Ray Siemens, and John Unsworth. [Link](http://digitalhumanities.org/companion/view?docId=blackwell/9781405103213/9781405103213.xml&doc.view=print&chunk.id=ss1-4-4&toc.depth=1&toc.id=0).

-   Krumme, Coco. “What Data Doesn’t Do.” In *Beautiful Data: The Stories behind Elegant Data Solutions*, edited by Toby Segaran and Jeff Hammerbacher, 1st ed. Beijing ; Sebastopol, CA: O’Reilly, 2009. [PDF](https://www.dropbox.com/s/b751c7noglf5nu0/Krumme%202009%20-%20What%20Data%20Doesn%27t%20Do.pdf?dl=0).

-   Manovich, Lev. “What Is Visualisation?” *Visual Studies* 26, no. 1 (March 15, 2011): 36–49. *http://www.tandfonline.com/doi/abs/10.1080/1472586X.2011.548488*. [PDF](https://www.dropbox.com/s/mb2vgfyvsqikh6b/Manovich%202011%20-%20What%20is%20Visualization%3F.pdf?dl=0).

-   Moretti, Franco. “Graphs.” In *Graphs, Maps, Trees: Abstract Models for Literary History*, 3–33. London ; New York: Verso, 2007. [PDF](https://www.dropbox.com/s/v7u7o3ni7a4pn5e/Moretti%202005%20-%20Graphs.pdf?dl=0).

-   McCandles, David. *Information is Beautiful*. *http://www.informationisbeautiful.net*



Optional Readings
-----------------

-   Gries, Stefan. “Useful statistics for corpus linguistics.”*<http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.160.9846&rep=rep1&type=pdf>

-   Thompson, Clive. “The Surprising History of the Infographic.” <http://www.smithsonianmag.com/history/surprising-history-infographic-180959563/?no-ist>

##### ▸ In-Class Outline


Week 8: Machine Learning
==========================


To Do Before Class
------------------

Choose an online data/metadata source, preferably the one you’re using for your final project. Using techniques from last week’s readings, present a quantitative exploration of the data using descriptive statistics and two or three visualizations. Up to two of these may be histograms, accompanied by another graphical format of your choice. You may use numerical values included in the collection or quantify some aspect of the data using techniques learned earlier in the course. In 300 words, describe your process and findings. Submit your code in a Jupyter notebook.

Install scipy Python library.

> pip install scipy

Install scikit-learn Python library and work through text classification tutorial.

> pip install sklearn
>
> pip install scikit-neuralnetwork


Readings
--------

-   Brew, Chris. “Language Processing: Statistical Methods.” In Encyclopedia of Language & Linguistics, edited by Keith Brown, 2nd ed., 12:597–604. Elsevier, 2006. [PDF](https://www.dropbox.com/s/s5tfn318otdvu3q/Brew%202006%20-%20Language%20Processing-%20Statistical%20Methods.pdf?dl=0).

-   “Working With Text Data.” scikit-learn.
                [http://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html](http://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html)

-   Geitgey, Adam. “Machine Learning is Fun!” *Medium*. [https://medium.com/@ageitgey/machine-learning-is-fun-80ea3ec3c471](https://medium.com/@ageitgey/machine-learning-is-fun-80ea3ec3c471)



Optional Readings
-----------------

-   Norvig, Peter. “Natural Language Corpus Data.” In *Beautiful Data: The Stories Behind Elegant Data Solutions*, edited by Toby Segaran and Jeff Hammerbacher, 1st ed. Beijing ; Sebastopol, CA: O’Reilly, 2009. [PDF](https://www.dropbox.com/s/6m8n6wzzd7887jp/Norvig%202009%20-%20Natural%20Language%20Corpus%20Data.pdf?dl=0).

-   Baharudin, Baharum, Lam Hong Lee, and Khairullah Khan. “A Review of Machine Learning Algorithms for Text-Documents Classification.” *Journal of Advances in Information Technology* 1, no. 1 (February 1, 2010). [PDF](https://www.dropbox.com/s/iljelruc17gvj0g/Khan%20et%20al.%202010%20-%20A%20Review%20of%20Machine%20Learning%20Algorithms%20for%20Text-Documents%20Classification.pdf?dl=0).



Topics to Cover
---------------

-   preprocessing for text machine learning:

    -   removing stop words

    -   lemmatizing

-   classifying texts using scikit-learn

-   author attribution

-   cluster analysis

##### ▸ In-Class Outline


Week 9: Critical Text Analysis
================================


To Do Before Class
------------------

Share your complete, cleaned dataset for the final project. In 200 words, describe the collection and the work you’ve done to shape and/or augment it. Submit a sample of your collection and/or processing code in a Jupyter notebook.

#### Reading

-   Hall, Gary. “Toward a Postdigital Humanities: Cultural Analytics and the Computational Turn to Data-Driven Scholarship.” *American Literature* 85, no. 4 (January 1, 2013): 781–809. [PDF](https://www.dropbox.com/s/d8ty5fcwm0afdtz/Hall%202013%20-%20Toward%20a%20Postdigital%20Humanities.pdf?dl=0).

-   Jockers, Matthew Lee. “Chapter 8: Theme.” In *Macroanalysis: Digital Methods and Literary History*, 118–53. Topics in the Digital Humanities. Urbana: University of Illinois Press, 2013. [PDF](https://www.dropbox.com/s/zsombfvplf5bh8f/Jockers%202013%20-%20Macroanalysis%20-%20Ch.%208%20-%20Theme.pdf?dl=0).

-   Marche, Stephen. “Literature Is not Data: Against Digital Humanities.” *Los Angeles Review of Books*, October 28th, 2012.
                [https://lareviewofbooks.org/essay/literature-is-not-data-against-digital-humanities](https://lareviewofbooks.org/essay/literature-is-not-data-against-digital-humanities)



Optional Reading
----------------

-   Ramsay, Stephen. “Chapter 3: Potential Readings.” In *Reading Machines: Toward an Algorithmic Criticism*, 33–57. Topics in the Digital Humanities. Urbana: University of Illinois Press, 2011. [PDF](https://www.dropbox.com/s/bo8dpeaodymk9d2/Ramsay%202011%20-%20Reading%20Machines%20-%20Ch.%203.pdf?dl=0).

-   Liu, Alan. “The Meaning of the Digital Humanities.” *PMLA* 128, no. 2 (March 2013): 409–23. [PDF](https://www.dropbox.com/s/avad81hqc5sp6iw/Liu%202013%20-%20The%20Meaning%20of%20the%20Digital%20Humanities.pdf?dl=0).

##### ▸ In-Class Outline


Week 10: Copyright and the Information Commons
================================================


To Do Before Class
------------------

Choose two machine learning algorithms discussed last week and a set of texts or metadata records, preferably the collection you are using for the final project. In 300–500 words, compare the likely efficacy of the two approaches and discuss how their classifications may differ.


Readings
--------

-   Sims, Nancy. “Library Licensing and Criminal Law: The Aaron Swartz Case.” *College & Research Libraries News* 72, no. 9 (2011): 534–37. [http://crln.acrl.org/content/72/9/534.short](http://crln.acrl.org/content/72/9/534.short).

-   O’Sullivan, Michael. “Aaron Swartz, New Technologies, and the Myth of Open Access.” In *Academic Barbarism, Universities and Inequality*. Palgrave Critical University Studies. Houndmills, Basingstoke, Hampshire ; New York, NY: Palgrave Macmillan, 2016. [Link](https://www.dropbox.com/s/xawj4hi4fpyj5mw/Aaron_Swartz_New_Technologies_and_the_My.docx?dl=0).

-   “The Digital Public Library of America Policy Statement on Metadata,” 2013. [http://dp.la/info/wp-content/uploads/2013/04/DPLAMetadataPolicy.pdf](http://dp.la/info/wp-content/uploads/2013/04/DPLAMetadataPolicy.pdf)

-   “Creative Commons: About the Licenses.” [https://creativecommons.org/licenses/](https://creativecommons.org/licenses/)

-   DRM article: [http://infojustice.org/wp-content/uploads/2015/03/band03102015.pdf](http://infojustice.org/wp-content/uploads/2015/03/band03102015.pdf)



Optional Readings
-----------------

-   Code of Best Practices in Fair Use for Academic and Research Libraries*. Association of Research Libraries, 2012*. [http://www.arl.org/storage/documents/publications/code-of-best-practices-fair-use.pdf](http://www.arl.org/storage/documents/publications/code-of-best-practices-fair-use.pdf)



Topics to Cover
---------------

-   copyright policy overview: DMCA, fair use, Creative Commons licenses

-   database copyright in the U.S. vs. Europe

-   legal debates around acquiring material for text and data mining research

##### ▸ In-Class Outline


Week 12: Peer Production & Crowdsourcing
========================================


To Do Before Class
------------------

Report your progress toward the final critical data analysis project in 300–500 words. Note your preliminary findings and describe how your perspective and/or approach has changed since you began.


Readings
--------

-   Benkler, Yochai. “Peer Production and Sharing.” In *The Wealth of Networks: How Social Production Transforms Markets and Freedom*, 59–90. New Haven [Conn.]: Yale University Press, 2006.

-   Manzo, Christina, Geoff Kaufman, Sukdith Punjasthitkul, and Mary Flanagan. “‘By the People, For the People’: Assessing the Value of Crowdsourced, User-Generated Metadata.” *Digital Humanities Quarterly* 9, no. 1 (2015). [http://www.digitalhumanities.org/dhq/vol/9/1/000204/000204.html](http://www.digitalhumanities.org/dhq/vol/9/1/000204/000204.html)

-   Bodó, Balázs. “Set the Fox to Watch the Geese: Voluntary IP Regimes in Piratical File-sharing Communities.” In Piracy: Leakages from Modernity, edited by James Arvanitakis and Martin Fredriksson, 241–63. Sacramento, CA: Litwin Books, 2014. [PDF](https://www.dropbox.com/s/3e2zrjiafp77pt9/Bodo%202014%20-%20Set%20the%20Fox%20to%20Watch%20the%20Geese.pdf?dl=0).

Optional Readings

-   Benkler, Yochai, and Helen Nissenbaum. “Commons-Based Peer Production and Virtue.” Journal of Political Philosophy 14, no. 4 (2006): 394–419. [https://www.nyu.edu/projects/nissenbaum/papers/jopp_235.pdf](https://www.nyu.edu/projects/nissenbaum/papers/jopp_235.pdf).

-   Kreiss, D., M. Finn, and F. Turner. “The Limits of Peer Production: Some Reminders from Max Weber for the Network Society.” New Media & Society 13, no. 2 (March 1, 2011): 243–59. [PDF](https://www.dropbox.com/s/mwhm10hz0nnania/Kreiss%20et%20al.%202011%20-%20The%20limits%20of%20peer%20production.pdf?dl=0).

##### ▸ In-Class Outline


*Week 14: Final Presentations*
------------------------------


*Sample Tools*
--------------

#### OpenRefine

Cleaning and transforming tabular data

-   [Installation instructions](https://github.com/OpenRefine/OpenRefine/wiki/Installation-Instructions)

-   Tutorials:

    -   [Tutorial: OpenRefine](http://casci.umd.edu/wp-content/uploads/2013/12/OpenRefine-tutorial-v1.5.pdf)

    -   [Video Tutorial 1: Introduction](https://www.youtube.com/watch?v=B70J_H_zAWM)

    -   [Video Tutorial 2: Data Transformation](https://www.youtube.com/watch?v=cO8NVCs_Ba0&nohtml5=False)

    -   [Video Tutorial 3: Data Augmentation](https://www.youtube.com/watch?v=5tsyz3ibYzk&nohtml5=False)
                    *

#### Fetch (FTP client)

-   [http://fetchsoftworks.com](http://fetchsoftworks.com)

-   shareware with *free licenses* for all students

#### JSON Parser Online

Browser-based tool for viewing JSON documents

- <http://json.parser.online.fr/beta/>

#### TextBlob: Simplified Text Processing

Python wrapper for NLTK and Pattern

- <https://textblob.readthedocs.org/en/dev/>

#### Beautiful Soup

Python module for parsing Web data

- <https://www.crummy.com/software/BeautifulSoup/>

#### Natural Language Toolkit

-   [Installation Instructions](http://www.nltk.org/install.html)

-   Tutorials:

    -   [Installing NLTK and Using it for Human Language Processing](https://www.howtoforge.com/tutorial/install-and-use-nltk-for-human-language-processing/)

    -   [Language Processing and Python](http://www.nltk.org/book/ch01.html)

    -   [Accessing Text Corpora and Lexical Resources](http://www.nltk.org/book/ch02.html)

    -   [Processing Raw Text](http://www.nltk.org/book/ch03.html)

    -   [NLTK HOWTOs](http://www.nltk.org/howto/)
                    *

#### Pattern

> Python module for web mining, NLP, machine learning, network analysis, and visualization.

- <http://www.clips.ua.ac.be/pattern>

#### PDFtk server

Command-line tool for editing PDF files.

- <https://www.pdflabs.com/tools/pdftk-server/>

#### ImageMagick

Command-line tool for editing and creating image files and PDFs.

- <http://www.imagemagick.org/script/index.php>

#### FFmpeg

Command-line tool for encoding and editing audio and video files.

- <https://ffmpeg.org/download.html>

#### SoX - Sound eXchange 

“The Swiss Army knife of sound processing programs”

- http://sox.sourceforge.net*



*Sample Data Sources
---------------------

#### Wordnik

A large collection of dictionary and thesaurus resources

-   [https://www.wordnik.com](https://www.wordnik.com/)

-   Python client for Wordnik API

    - <https://github.com/wordnik/wordnik-python>
        *

#### WordNet

> Lexical database from Princeton University containing synonyms, antonyms, and other logical relationships among words

- <http://wordnet.princeton.edu>

#### Project Gutenberg

50,000+ electronic books in a variety of formats

- [https://www.gutenberg.org](https://www.gutenberg.org/)

#### Folger Digital Texts

> Shakespeare’s complete works with rich metadata, in a variety of machine- and human-readable formats

-   [http://www.folgerdigitaltexts.org/](http://www.folgerdigitaltexts.org/)

-   Ullyot, Michael, "Mark me: Using the Folger Digital Texts," *Spenser Review* 44.1.7 (Spring–Summer 2014). [http://www.english.cam.ac.uk/spenseronline/review/volume-44/441/digital-projects/folger-digital-texts](http://www.english.cam.ac.uk/spenseronline/review/volume-44/441/digital-projects/folger-digital-texts)

#### Wikidata 

A collection of linked data from Wikipedia and other Wikimedia projects

-   Wikidata Tours

    -   [https://www.wikidata.org/wiki/Wikidata:Tours](https://www.wikidata.org/wiki/Wikidata:Tours)

-   “An Ambitious Wikidata Tutorial”

    -   [http://www.slideshare.net/_Emw/an-ambitious-wikidata-tutorial](http://www.slideshare.net/_Emw/an-ambitious-wikidata-tutorial)

#### NYPL Digital Collections API

> Access to 1 million digitized items from the New York Public Library (requires application approval)

- [http://api.repo.nypl.org](http://api.repo.nypl.org/)

#### Cooper Hewitt Collection

> Metadata and image links for 75% of the collection at Cooper Hewitt, Smithsonian Design Museum

-   [https://github.com/cooperhewitt/collection](https://github.com/cooperhewitt/collection)

-   API: <https://collection.cooperhewitt.org/api/>

#### Open Data at the New York Philharmonic

Metadata for 20,000+ orchestral performances and 500,000+ subscriber records

- <http://archives.nyphil.org/index.php/open-data>

#### The Tate Collection

Metadata on ~70,000 artworks and ~3,500 artists from the UK’s Tate collection

- <https://github.com/tategallery/collection>

#### Victoria and Albert Museum Collection

> API access to metadata for 1.1M+ objects and 375K+ images from the Victoria and Albert Museum, London

- <http://www.vam.ac.uk/api/>

#### Genius API

- <https://docs.genius.com/>

#### Google Books API

- [Working with Volumes](https://developers.google.com/books/docs/v1/using#WorkingVolumes)

#### Open Library

Metadata for 20M+ books and 6M+ authors, available for bulk download and API access

-   [https://openlibrary.org/data](https://openlibrary.org/data)

#### ISBN+ Open Source ISBN Database

Metadata for 10M+ books, accessible via API

- [http://isbnplus.com](http://isbnplus.com/)

#### HathiTrust Data API

> Access to metadata, page images, and OCR text from millions of public-domain books in the HathiTrust Digital Library

- <https://www.hathitrust.org/data_api>

#### Music Brainz Database

Volunteer-run database of metadata for 15M+ tracks, 12M+ albums, and 700K+ artists

- <http://musicbrainz.org/doc/MusicBrainz_Database>

#### Million Song Dataset

Metadata and extracted audio features for 1M+ songs

- <http://labrosa.ee.columbia.edu/millionsong/>

#### Supreme Court Decisions

- <https://www.law.cornell.edu/supremecourt/text/home>

#### Pro Publica Data

Public datasets including collections related to education, healthcare, and politics

-   [https://www.propublica.org/data/](https://www.propublica.org/data/)

### Lists of Public Data Sources

#### APIs for Scholarly Resources

- <http://libguides.mit.edu/apis>

#### Culture Hack

-   [http://data.culturehack.org.uk](http://data.culturehack.org.uk/)

#### “Data, Data, Data: Thousands of Public Data Sources”

- <https://blog.bigml.com/2013/02/28/data-data-data-thousands-of-public-data-sources/>

#### Datasets for Data Mining and Data Science

- <http://www.kdnuggets.com/datasets/index.html>

#### List of Public Data Sources Fit for Machine Learning

- <https://blog.bigml.com/list-of-public-data-sources-fit-for-machine-learning/#various_lists>

#### AWS Public Data Sets

-   [https://aws.amazon.com/datasets/](https://aws.amazon.com/datasets/)

#### “A collection of museum, gallery, library, archive, archaeology and cultural heritage APIs, machine-readable, linked and open data services for open cultural data”

- <http://museum-api.pbworks.com/w/page/21933420/Museum%C2%A0APIs>

#### Quora: “Where can I find large datasets open to the public?”

-   [http://www.quora.com/Where-can-I-find-large-datasets-open-to-the-public](http://www.quora.com/Where-can-I-find-large-datasets-open-to-the-public)

#### Reddit: “What are some fun API's to play with?”

-   <https://www.reddit.com/r/webdev/comments/3wrswc/what_are_some_fun_apis_to_play_with>


