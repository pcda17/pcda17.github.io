
Syllabus: Programming for Cultural Data Analysis
====================================================
Fall 2017, Mondays 3-6pm

Instructor: Tanya Clement 
TA: Steve McLaughlin

University of Texas at Austin School of Information

- [Tools and Datasets](tools_data.md)

- In-Class Outlines:

[Week 1](week-01.md) | [Week 2](week-02.md) | [Week 3](week-03.md) | [Week 4](week-04.md) | [Week 5](week-05.md)
[Week 6](week-06.md) | [Week 7](week-07.md) | [Week 8](week-08.md) | [Week 9](week-09.md) | [Week 10](week-10.md)
| [Week 11](week-11.md) | [Week 12](week-12.md)

### Course Objectives

Prerequsites: advanced-level undergraduate or graduate coursework in the humanities; no or very little programming experience preferred; 

In the data, information, knowledge, wisdom (DIKW) hierarchy that circulates through Knowledge Management (KM) and Information Science (IS) discussions, *data* appears at the base of a pyramid of which wisdom is the pinnacle. In this schematic, *data* is “raw” and lacking in meaning, while *information*, the next higher level of the pyramid---just below *knowledge* and then *wisdom*---represents the presence of added links and relationships; *information* is higher up on the wisdom chain because it is *data* made meaningful. In the humanities, students are taught that data is not found in the “raw” but has rather been cooked all along, taken and constructed and seasoned according to our situated contexts including access issues (*Where* is the data?); media, format, and technology constraints (*How* is the data?); and perspectives (*What* is the data? *Who* is involved in and impacted by its creation and use?). 

Learning to think critically about data as *information* means rejecting common illusions about data more generally, including its objectivity, impersonality, atemporality, and authorlessness. To teach students to think about *information* from this more critical perspective means first understanding how a culture tends to understand what is informative. 

Towards these ends, this course takes on "data wrangling" in the context of humanist perspectives. 

Goals: 
 
-   Teach scripting-style programming in Python and Unix-like systems, emphasizing literacy in finding and using free and open source software.

-   Familiarize students with techniques for collecting, transforming, and analyzing media and metadata available on the Web.

-   Introduce commonly used data models and their standard formats, including CSV, JSON, and XML.

-   Explore computational text analysis techniques such as natural language processing (NLP), sentiment analysis, and machine learning classification.

-   Introduce tools for analyzing cultural data via visualization and statistical tests, emphasizing critical reflection on the limitations of these approaches.

-   Familiarize students with Web archiving and data curation practices.

-   Explore cultural implications of large-scale preservation of cultural materials.


### Course Principles

-  Writing critically about data requires both a level of knowldege about data and data wrangling as it requires a level of knowledge about thinking and writing from critical perspectives learned in cultural studies. While this course does not *teach* cultural studies, an understanding of and experience in humanities theory and research and the principles of cultural studies are essential. 

-  Imitating and modifying others’ code is essential in learning to program. You can many examples and explanations on [Stack Exchange](http://stackexchange.com) and similar online forums. Taking one or two lines without attribution is OK; if you use a longer chunk of code found online, add a #comment with the source’s URL.

-   Begin assignments early. If you realize what you had in mind is more difficult than expected, talk to the instructor about choosing an alternative.

-   We’ll be focusing on a scripting approach to programming. This course is not oriented toward developing large, complex programs or writing perfectly optimized code.

-   Learning to code takes trial and error. Work through weekly programming tutorials before class and continue polishing in-class coding assignments at home.

## Assignments

### Final Project: Critical Data Analysis (50%)

For your final project, you will use a dataset drawn from online sources and analyze those data in a critical essay. You may either present an argument about the data (e.g., describing bias in the way the data were chosen and arranged) or you may use your dataset as the basis for an argument about culture (e.g., tracing a stylistic shift in a literary community). You should conceive and execute your project with a specific audience in mind, such as literary scholars, newspaper readers, or policy advocates.

Your dataset should comprise at least 200 texts or other media files, or at least 2000 metadata records. The size of your collection should be appropriate to your technical skills and the complexity of each record. Rather than using an entire pre-existing dataset, you may choose to extend or limit the dataset in some way. This might mean curating material from multiple sources, mashing up two or more datasets, augmenting records using machine learning or natural language processing, or using a creative technique to organize messy data.

Your final project will include the following elements:

-   Proposal (7%)

-   Proposal Peer Review (3%)

-   In-class presentation (week 14) (10%)

-   12 page critical essay, with an appendix of 3–4 data visualizations (30%)

### Weekly Assignments (WA) (50%)

Except when indicated, there will be required readings each week. The required readings will either be available online and linked below or posted on Canvas, so there are no books to buy or papers to acquire for the class.

Assignments should be posted on Canvas by midnight the day before class. 

### Resources

-   Software Tools

-   Sample Data Sources

##### ▸ In-Class Outline

Week 1 (9/11): Introductions & Command Line Basics
===========================================

To Do Before Class
------------------
To access Lynda videos, follow links below, click “Log in,” then “Organizational Login,” and enter your UT EID and password.

- Optional: Allardice, Simon. “Foundations of Programming: Fundamentals.” Lynda.com. [http://www.lynda.com/JavaScript-tutorials/Foundations-of-Programming-Fundamentals/83603-2.html](http://www.lynda.com/JavaScript-tutorials/Foundations-of-Programming-Fundamentals/83603-2.html)

- Optional: Marini, Joe. “Up and Running with Python.” Lynda.com.
            [http://www.lynda.com/Python-tutorials/Welcome/122467/142550-4.html](http://www.lynda.com/Python-tutorials/Welcome/122467/142550-4.html)

## Software to install before class

- Text editor: Atom or Geany
    - [https://atom.io](https://atom.io)
    - [https://www.geany.org](https://www.geany.org)

- Docker Community Edition or Docker Toolbox
    - [Docker CE](https://store.docker.com/search?type=edition&offering=community) (macOS/Linux)
    - [Docker Toolbox](https://www.docker.com/products/docker-toolbox) (Windows)

- VLC Media Player
    - [https://www.videolan.org/vlc/](https://www.videolan.org/vlc/)


Readings
-------
-   Montfort, Nick. “Why Program?” In *Exploratory Programming for the Arts and Humanities*, 267–77. Cambridge, MA: The MIT Press, 2016. [PDF](https://www.dropbox.com/s/kb2xy8giavxpo89/Montfort%202016%20-%20Why%20Program.pdf?dl=0).

-   danah boyd & Kate Crawford (2012) CRITICAL QUESTIONS FOR BIG DATA, Information, Communication & Society, 15:5, 662-679

To start for next week:
-   Stephenson, Neal. “In the Beginning Was the Command Line.” Cryptonomicon, 1999. [Note: This reading is due the second week of the course but it's quite long] <http://www.cryptonomicon.com/beginning.html>. [TXT](http://www.cryptonomicon.com/command.zip). [PDF](https://www.dropbox.com/s/kbpvllkmlb7u5uh/Neal%20Stephenson%201999%20-%20In%20the%20Beginning%20was%20the%20Command%20Line.pdf?dl=1). [EPUB](https://www.dropbox.com/s/sisnsmw0m0b6vci/Neal%20Stephenson%201999%20-%20In%20the%20Beginning%20was%20the%20Command%20Line.epub?dl=0).

##### ▸ In-Class Outline


Week 2 (9/18): The Operating System in Context
==========================================

To Do Before Class
------------------
Read pages 1–28 of Shieber’s Python tutorial and work through the code examples.
-   Shieber, Stuart M., *Programming for Humanists* pages 1–28, 2014. [http://blogs.harvard.edu/programmingforhumanists/files/2014/12/proghum.pdf](http://blogs.harvard.edu/programmingforhumanists/files/2014/12/proghum.pdf)

Work through Chris Albon’s tutorial on Python string operations.
-   Albon, Chris. “String Operations.” [http://chrisalbon.com/python/string_operations.html](http://chrisalbon.com/python/string_operations.html)


Readings
-------
-   Noria, Xavier. “Understanding Newlines.” *O’Reilly ONLamp*, August 17, 2006. [http://www.onlamp.com/pub/a/onlamp/2006/08/17/understanding-newlines.html](http://www.onlamp.com/pub/a/onlamp/2006/08/17/understanding-newlines.html)

-   Oualline, Steve. “The End of Line Puzzle.” *The Practical Programmer*. [http://www.oualline.com/practical.programmer/eol.html](http://www.oualline.com/practical.programmer/eol.html)

-   Stephenson, Neal. “In the Beginning Was the Command Line.” Cryptonomicon, 1999. <http://www.cryptonomicon.com/beginning.html>. [TXT](http://www.cryptonomicon.com/command.zip). [PDF](https://www.dropbox.com/s/kbpvllkmlb7u5uh/Neal%20Stephenson%201999%20-%20In%20the%20Beginning%20was%20the%20Command%20Line.pdf?dl=1). [EPUB](https://www.dropbox.com/s/sisnsmw0m0b6vci/Neal%20Stephenson%201999%20-%20In%20the%20Beginning%20was%20the%20Command%20Line.epub?dl=0).

Asssignment
-------
[WA #1](https://utexas.instructure.com/courses/1204381/discussion_topics/2826310)

##### ▸ In-Class Outline

Week 3 (9/25): Collections as Data: Meaning making
================================

To Do Before Class
------------------
-   “The Jupyter Notebook.” [http://jupyter-notebook.readthedocs.io/en/latest/notebook.html](http://jupyter-notebook.readthedocs.io/en/latest/notebook.html)

Readings
--------
- Gallinger, M. and Daniel Chudnov "Library of Congress Lab: Library of Congress Digital Scholars Lab Pilot Project Report," ([PDF](http://digitalpreservation.gov/meetings/dcs16/DChudnov-MGallinger_LCLabReport.pdf).

- Introna, L. D. “The Enframing of Code: Agency, Originality and the Plagiarist.” *Theory, Culture & Society* 28, no. 6 (November 1, 2011): 113–41. [PDF](https://www.dropbox.com/s/s0zmg1iw308vb4e/Introna%202011%20-%20The%20Enframing%20of%20Code-%20Agency%2C%20Originality%20and%20the%20Plagiarist.pdf?dl=0).

- Padilla, T. "On a Collections as Data Imperative." [PDF](http://digitalpreservation.gov/meetings/dcs16/tpadilla_OnaCollectionsasDataImperative_final.pdf).

-   Posner, Miriam. “Humanities Data: A Necessary Contradiction.” *Miriam Posner’s Blog*, June 25, 2015. *http://miriamposner.com/blog/humanities-data-a-necessary-contradiction*

Asssignment
--------
[WA #2](https://utexas.instructure.com/courses/1204381/discussion_topics/2840058)

##### ▸ In-Class Outline

Week 4 (10/2): Collections as Data: Data Models
===================

To Do Before Class
------------------
Readings
--------

-   Albon, Chris. “Parse JSON File.” [http://chrisalbon.com/python/json_parse_file.html](http://chrisalbon.com/python/json_parse_file.html)

-   van Hooland, Seth, and Ruben Verborgh. “Modelling.” In *Linked Data for Libraries, Archives and Museums: How to Clean, Link and Publish Your Metadata*, 11–70. Chicago: Neal-Schuman, 2014. [PDF](https://www.dropbox.com/s/uv9xhmiq574rbyj/van%20Hooland%20and%20Verborgh%202014%20-%20Modelling.pdf?dl=0).

-   Zhuang, Atima Han, Ishita Vedvyas, and Rishikesh Dole. “Tutorial: OpenRefine,” 2013. [http://casci.umd.edu/wp-content/uploads/2013/12/OpenRefine-tutorial-v1.5.pdf](http://casci.umd.edu/wp-content/uploads/2013/12/OpenRefine-tutorial-v1.5.pdf)


Optional Readings
-----------------

-   Fortune, Stephen. “A Brief History of Databases.” *Avant*, February 27th 2014. [https://web.archive.org/web/20150220031213/http://avant.org/media/history-of-databases](https://web.archive.org/web/20150220031213/http://avant.org/media/history-of-databases)

-   Lundh, Fredrik. “Elements and Element Trees.” [http://effbot.org/zone/element.htm](http://effbot.org/zone/element.htm) [Python XML tutorial]

-   Beazley, David, and Brian K. Jones. “Chapter 6: Data Encoding and Processing.” In Python Cookbook: *recipes for Mastering Python 3*, 3. ed., 175–216. Bejing: O’Reilly, 2013. [PDF](https://www.dropbox.com/s/2dp0ylqlpsp6czr/Python_Cookbook_3rd-ed_Ch-6.pdf?dl=1)

Asssignment
--------
[WA #3](https://utexas.instructure.com/courses/1204381/discussion_topics/2841839)

##### ▸ In-Class Outline

Week 5 (10/9): Word-Level Text Analysis
================================

To Do Before Class
------------------

Install textblob package before class (a wrapper for NLTK and pattern) and work through Montfort’s code examples. The --user option lets us install a module for the current user only, without requiring an admin password.

> pip install --user -U textblob
>
> python -m textblob.download_corpora


Readings
--------
-   Ramsay, Stephen. “Chapter 1: An Algorithmic Criticism.” In *Reading Machines: Toward an Algorithmic Criticism*, 1–17. Topics in the Digital Humanities. Urbana: University of Illinois Press, 2011. [PDF](https://www.dropbox.com/s/ox35us0vfj7ppng/Ramsay%202011%20-%20Reading%20Machines%20-%20Ch.%201.pdf?dl=0).

-   Montfort, Nick. “Text III.” In *Exploratory Programming for the Arts and Humanities*, 185–213. Cambridge, MA: The MIT Press, 2016. [PDF](https://www.dropbox.com/s/gib77npezdaz1kr/Montfort%202016%20-%20Text%20III.pdf?dl=0).

-   Fellenbaum, Christiane. “Wordnet(s).” In The *Encyclopedia of Language & Linguistics*, edited by E. K. Brown and Anne Anderson, 2nd ed., 14:665–79. Amsterdam ; Boston: Elsevier, 2005. [PDF](https://www.dropbox.com/s/zxuvhzlheiyo7uc/Fellenbaum%202005%20-%20Wordnet%28s%29.pdf?dl=0).

-   “Alphabetical list of part-of-speech tags used in the Penn Treebank Project.” [https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html](https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html)


Asssignment
--------
[WA #4](https://utexas.instructure.com/courses/1204381/discussion_topics/2841813)

##### ▸ In-Class Outline


Week 6 (10/16): Web Scraping & APIs
=============================

To Do Before Class
-------------------

Install [Beauitful Soup](https://www.crummy.com/software/BeautifulSoup/) library for parsing HTML.

> pip install -U --user beautifulsoup

Work through Chris Albon’s Beautiful Soup tutorial.

Readings
--------
-   Pomerantz, Jeffrey. “The Future of Metadata.” In *Metadata*. The MIT Press Essential Knowledge Series. Cambridge, MA ; London, England: The MIT Press, 2015. [PDF](https://www.dropbox.com/s/hj3i12cinl3ublj/Pomerantz%202015%20-%20Ch.%208%20-%20The%20Future%20of%20Metadata.pdf?dl=0).

-   Swartz, Aaron. “Building a Platform: Providing APIs.” In *Aaron Swartz’s ‘A Programmable Web’: An Unfinished Work*, 31–39. San Rafael, CA: Morgan & Claypool Publishers, 2013. [PDF](https://www.dropbox.com/s/wmgtcko0u9q59aw/Swartz%202013%20-%20Building%20a%20Platform-%20Providing%20APIs.pdf?dl=0).

-   Kelly, Chelsea Emelie. “Beyond Digital: Open Collections & Cultural Institutions,” 2014. *https://artmuseumteaching.com/2014/11/06/beyond-digital-open-collections-cultural-institutions*

-   “HTML Introduction” and “HTML5 Introduction.” W3Schools.

    -   [http://www.w3schools.com/html/html_intro.asp](http://www.w3schools.com/html/html_intro.asp)

    -   [http://www.w3schools.com/html/html5_intro.asp](http://www.w3schools.com/html/html5_intro.asp)

-   Albon, Chris. “Beautiful Soup Basic HTML Scraping.” [http://chrisalbon.com/python/beautiful_soup_html_basics.html](http://chrisalbon.com/python/beautiful_soup_html_basics.html)


Optional Readings
-----------------
-   Sanger, David E., and Eric Schmitt. “Snowden Used Low-Cost Tool to Best N.S.A.” The New York Times. February 8, 2014. [http://www.nytimes.com/2014/02/09/us/snowden-used-low-cost-tool-to-best-nsa.html](http://www.nytimes.com/2014/02/09/us/snowden-used-low-cost-tool-to-best-nsa.html)

-   Kazil, Jacqueline, and Katharine Jarmul. “PDFs and Problem Solving in Python.” In *Data Wrangling with Python: Tips and Tools to Make Your Life Easier*, 91–126. O’Reilly, 2016. [PDF](https://www.dropbox.com/s/hfc8m731eiik0g8/Kazil%20and%20Jarmul%202016%20-%20PDFs%20and%20Problem%20Solving%20in%20Python.pdf?dl=0).

Asssignment
--------
[WA #5](https://utexas.instructure.com/courses/1204381/discussion_topics/2841854)

##### ▸ In-Class Outline


Week 7 (10/23) The Politics of Data
=========================

To Do Before Class
------------------
Readings
--------
-  Christen, Kim. “Does Information Really Want to be Free? Indigenous Knowledge Systems and the Question of Openness.” International Journal of Communication 6 (2012), 2870–2893.

-   Peters, Justin. *The Idealist: Aaron Swartz and the Rise of Free Culture on the Internet*, Chapters 7 and 8. New York: Scribner, 2016. [PDF](https://www.dropbox.com/s/fg195av2ayiwc31/Peters%202016%20-%20The%20Idealist%20-%20Chs.%206-7.pdf?dl=0).

-   Greenwald, Glenn. “Chapter 1: Contact.” In *No Place to Hide: Edward Snowden, the NSA, and the U.S. Surveillance State*, 2015. [PDF](https://www.dropbox.com/s/1evnc6xu6pbdin6/Greenwald%202014%20-%20No%20Place%20to%20Hide%20-%20Intro%20%26%20Chapter%201.pdf?dl=0).

-   Freelon, Deen Goodwin, Charlton D. McIlwain, and Meredith D. Clark. “Beyond the Hashtags: #Ferguson, #Blacklivesmatter, and the Online Struggle for Offline Justice,” 2016. [http://cmsimpact.org/wp-content/uploads/2016/03/beyond_the_hashtags_2016.pdf](http://cmsimpact.org/wp-content/uploads/2016/03/beyond_the_hashtags_2016.pdf)

-   American Civil Liberties Union. "First Amendment Lawsuit Brought on Behalf of Academic Researchers and Journalists Who Fear Prosecution Under the Computer Fraud and Abuse Act." [https://www.aclu.org/news/aclu-challenges-law-preventing-studies-big-data-discrimination](https://www.aclu.org/news/aclu-challenges-law-preventing-studies-big-data-discrimination)

Optional Readings
-----------------
-   Day, Ronald E. “Governing Expression: Social Big Data and Neoliberalism.” In *Indexing It All: The Subject in the Age of Documentation*, Information, and Data, 123–44. History and Foundations of Information Science. Cambridge, Massachusetts: The MIT Press, 2014. [PDF](https://www.dropbox.com/s/mab080ymg2pqjon/Day%202014%20-%20Indexing%20it%20All%20-%20Ch.%206%20-%20Governing%20Expression-%20Social%20Big%20Data%20and%20Neoliberalism.pdf?dl=0).

-   Hitchcock, Tim. “Digital Searching and the Re-formulation of Historical Knowledge” 2008. In *The Virtual Representation of the Past*, edited by Mark Greenglass and Lorna Hughes, 81-90. Ashgate: 2008. [PDF](https://www.dropbox.com/s/ht8si4vygm3bkh4/Hitchcock%202008%20-%20Digital%20Searching%20and%20the%20Re-formulation%20of%20Historical%20Knowledge.pdf?dl=0).

Asssignment
--------
[WA #6](https://utexas.instructure.com/courses/1204381/discussion_topics/2841926) 

##### ▸ In-Class Outline


Week 8 (10/30): Your Data
=========================
To Do Before Class
------------------
Readings
--------
-   Winner, Langdon. “Do Artifacts Have Politics?” *Daedalus* 109, no. 1 (1980): 121–36. [PDF](https://www.dropbox.com/s/ttr620gqbv4tj48/Winner%201980%20-%20Do%20Artifacts%20Have%20Politics%3F.pdf?dl=0).

-   Joerges, B. “Do Politics Have Artefacts?” *Social Studies of Science* 29, no. 3 (June 1, 1999): 411–31. [PDF](https://www.dropbox.com/s/mb8cn5trvphm3oz/Joerges%201999%20-%20Do%20Politics%20Have%20Artefacts.pdf?dl=0).

-   Sacasas, Michael. “Do Artifacts Have Ethics?” *The Frailest Thing*, November 29, 2014. [http://thefrailestthing.com/2014/11/29/do-artifacts-have-ethics](http://thefrailestthing.com/2014/11/29/do-artifacts-have-ethics/)


Asssignment
--------
[Due: Proposal](https://utexas.instructure.com/courses/1204381/assignments/4166696) 


##### ▸ In-Class Outline

Week 9 (11/6): Statistics and Visualization
====================================

To Do Before Class
------------------

Install [numpy](http://www.numpy.org/) scientific computing library for Python.

> pip install --user -U numpy

Install [pandas](http://pandas.pydata.org/) data analysis library for Python.

> pip install --user -U pandas

Install [matplotlib](http://matplotlib.org/) visualization library for Python.

> pip install --user -U matplotlib

Readings
--------
-   Montfort, Nick. Excerpt from “Statistics and Visualization.” In *Exploratory Programming for the Arts and Humanities*, 215–40. Cambridge, MA: The MIT Press, 2016. [PDF](https://www.dropbox.com/s/7ihzxmrcq2997e4/Montfort%202016%20-%20Statistics%20and%20Visualization.pdf?dl=0).

-   Krumme, Coco. “What Data Doesn’t Do.” In *Beautiful Data: The Stories behind Elegant Data Solutions*, edited by Toby Segaran and Jeff Hammerbacher, 1st ed. Beijing ; Sebastopol, CA: O’Reilly, 2009. [PDF](https://www.dropbox.com/s/b751c7noglf5nu0/Krumme%202009%20-%20What%20Data%20Doesn%27t%20Do.pdf?dl=0).

-   Manovich, Lev. “What Is Visualisation?” *Visual Studies* 26, no. 1 (March 15, 2011): 36–49. *http://www.tandfonline.com/doi/abs/10.1080/1472586X.2011.548488*. [PDF](https://www.dropbox.com/s/mb2vgfyvsqikh6b/Manovich%202011%20-%20What%20is%20Visualization%3F.pdf?dl=0).

-   Moretti, Franco. “Graphs.” In *Graphs, Maps, Trees: Abstract Models for Literary History*, 3–33. London ; New York: Verso, 2007. [PDF](https://www.dropbox.com/s/v7u7o3ni7a4pn5e/Moretti%202005%20-%20Graphs.pdf?dl=0).

-   McCandles, David. *Information is Beautiful*. *http://www.informationisbeautiful.net*


Optional Readings
-----------------
-   Gries, Stefan. “Useful statistics for corpus linguistics.”*<http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.160.9846&rep=rep1&type=pdf>

-   Thompson, Clive. “The Surprising History of the Infographic.” <http://www.smithsonianmag.com/history/surprising-history-infographic-180959563/?no-ist>

Asssignment
--------
[Due: Proposal Peer Review](https://utexas.instructure.com/courses/1204381/assignments/4166696).


##### ▸ In-Class Outline


Week 10 (11/13): Machine Learning
==========================
To Do Before Class
------------------
Readings
--------
-   Brew, Chris. “Language Processing: Statistical Methods.” In Encyclopedia of Language & Linguistics, edited by Keith Brown, 2nd ed., 12:597–604. Elsevier, 2006. [PDF](https://www.dropbox.com/s/s5tfn318otdvu3q/Brew%202006%20-%20Language%20Processing-%20Statistical%20Methods.pdf?dl=0).

-   Julia Angwin, Jeff Larson, Surya Mattu and Lauren Kirchner, ProPublica. “Machine Bias.” *ProPublica*. May 23, 2016. [https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)

-   “Working With Text Data.” scikit-learn.
                      [http://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html](http://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html)

-   Geitgey, Adam. “Machine Learning is Fun!” *Medium*. [https://medium.com/@ageitgey/machine-learning-is-fun-80ea3ec3c471](https://medium.com/@ageitgey/machine-learning-is-fun-80ea3ec3c471)

Optional Readings
-----------------
-   Norvig, Peter. “Natural Language Corpus Data.” In *Beautiful Data: The Stories Behind Elegant Data Solutions*, edited by Toby Segaran and Jeff Hammerbacher, 1st ed. Beijing ; Sebastopol, CA: O’Reilly, 2009. [PDF](https://www.dropbox.com/s/6m8n6wzzd7887jp/Norvig%202009%20-%20Natural%20Language%20Corpus%20Data.pdf?dl=0).

-   Baharudin, Baharum, Lam Hong Lee, and Khairullah Khan. “A Review of Machine Learning Algorithms for Text-Documents Classification.” *Journal of Advances in Information Technology* 1, no. 1 (February 1, 2010). [PDF](https://www.dropbox.com/s/iljelruc17gvj0g/Khan%20et%20al.%202010%20-%20A%20Review%20of%20Machine%20Learning%20Algorithms%20for%20Text-Documents%20Classification.pdf?dl=0).


Asssignment
--------
Install scipy Python library.

> pip install scipy

Install scikit-learn Python library and work through text classification tutorial.

> pip install sklearn
>
> pip install scikit-neuralnetwork

WA #7: Use some of the techniques from last week’s readings on the online/data source that you have identified for your final project;  present a quantitative exploration of the data using descriptive statistics and two or three visualizations. Up to two of these may be histograms, accompanied by another graphical format of your choice. You may use numerical values included in the collection or quantify some aspect of the data using techniques learned earlier in the course. Reflect on your process and findings through this weeks' readings, specifically in relation to Burrows. Submit your code in a Jupyter notebook.

##### ▸ In-Class Outline


Week 11 (11/20): Critical Text Analysis
================================
To Do Before Class
------------------
Readings
--------
-   Burrows, John. “Textual Analysis.” In *Companion to Digital Humanities*, edited by Susan Schreibman, Ray Siemens, and John Unsworth. [Link](http://digitalhumanities.org/companion/view?docId=blackwell/9781405103213/9781405103213.xml&doc.view=print&chunk.id=ss1-4-4&toc.depth=1&toc.id=0).

-   Hall, Gary. “Toward a Postdigital Humanities: Cultural Analytics and the Computational Turn to Data-Driven Scholarship.” *American Literature* 85, no. 4 (January 1, 2013): 781–809. [PDF](https://www.dropbox.com/s/d8ty5fcwm0afdtz/Hall%202013%20-%20Toward%20a%20Postdigital%20Humanities.pdf?dl=0).

-   Jockers, Matthew Lee. “Chapter 8: Theme.” In *Macroanalysis: Digital Methods and Literary History*, 118–53. Topics in the Digital Humanities. Urbana: University of Illinois Press, 2013. [PDF](https://www.dropbox.com/s/zsombfvplf5bh8f/Jockers%202013%20-%20Macroanalysis%20-%20Ch.%208%20-%20Theme.pdf?dl=0).

-   Marche, Stephen. “Literature Is not Data: Against Digital Humanities.” *Los Angeles Review of Books*, October 28th, 2012.
                      [https://lareviewofbooks.org/essay/literature-is-not-data-against-digital-humanities](https://lareviewofbooks.org/essay/literature-is-not-data-against-digital-humanities)

Optional Reading
----------------
-   Ramsay, Stephen. “Chapter 3: Potential Readings.” In *Reading Machines: Toward an Algorithmic Criticism*, 33–57. Topics in the Digital Humanities. Urbana: University of Illinois Press, 2011. [PDF](https://www.dropbox.com/s/bo8dpeaodymk9d2/Ramsay%202011%20-%20Reading%20Machines%20-%20Ch.%203.pdf?dl=0).

-   Liu, Alan. “The Meaning of the Digital Humanities.” *PMLA* 128, no. 2 (March 2013): 409–23. [PDF](https://www.dropbox.com/s/avad81hqc5sp6iw/Liu%202013%20-%20The%20Meaning%20of%20the%20Digital%20Humanities.pdf?dl=0).

Asssignment
--------
WA #8:  Share your complete, cleaned dataset for the final project. In 200 words, describe the collection and the work you’ve done to shape and/or augment it. Submit a sample of your collection and/or processing code in a Jupyter notebook.

##### ▸ In-Class Outline


Week 12 (11/27): Copyright and the Information Commons
================================================
To Do Before Class
------------------
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


Asssignment
--------
WA #9:  Choose two machine learning algorithms discussed last week and a set of texts or metadata records, preferably the collection you are using for the final project. In 300–500 words, compare the likely efficacy of the two approaches and discuss how their classifications may differ.


##### ▸ In-Class Outline


Week 13 (12/4): Peer Production & Crowdsourcing
========================================
To Do Before Class
------------------
Readings
--------
-   Benkler, Yochai. “Peer Production and Sharing.” In *The Wealth of Networks: How Social Production Transforms Markets and Freedom*, 59–90. New Haven [Conn.]: Yale University Press, 2006.

-   Manzo, Christina, Geoff Kaufman, Sukdith Punjasthitkul, and Mary Flanagan. “‘By the People, For the People’: Assessing the Value of Crowdsourced, User-Generated Metadata.” *Digital Humanities Quarterly* 9, no. 1 (2015). [http://www.digitalhumanities.org/dhq/vol/9/1/000204/000204.html](http://www.digitalhumanities.org/dhq/vol/9/1/000204/000204.html)

-   Bodó, Balázs. “Set the Fox to Watch the Geese: Voluntary IP Regimes in Piratical File-sharing Communities.” In Piracy: Leakages from Modernity, edited by James Arvanitakis and Martin Fredriksson, 241–63. Sacramento, CA: Litwin Books, 2014. [PDF](https://www.dropbox.com/s/3e2zrjiafp77pt9/Bodo%202014%20-%20Set%20the%20Fox%20to%20Watch%20the%20Geese.pdf?dl=0).

Optional Readings
--------
-   Benkler, Yochai, and Helen Nissenbaum. “Commons-Based Peer Production and Virtue.” Journal of Political Philosophy 14, no. 4 (2006): 394–419. [https://www.nyu.edu/projects/nissenbaum/papers/jopp_235.pdf](https://www.nyu.edu/projects/nissenbaum/papers/jopp_235.pdf).

-   Kreiss, D., M. Finn, and F. Turner. “The Limits of Peer Production: Some Reminders from Max Weber for the Network Society.” New Media & Society 13, no. 2 (March 1, 2011): 243–59. [PDF](https://www.dropbox.com/s/mwhm10hz0nnania/Kreiss%20et%20al.%202011%20-%20The%20limits%20of%20peer%20production.pdf?dl=0).

Asssignment
--------
WA #10:   Report your progress toward the final critical data analysis project in 300–500 words. Note your preliminary findings and describe how your perspective and/or approach has changed since you began.

##### ▸ In-Class Outline


*Week 14 (12/11): Final Presentations*
========================================
[Final Presentation due](https://utexas.instructure.com/courses/1204381/assignments/4166564)

12/18: [Final Project due](https://utexas.instructure.com/courses/1204381/assignments/4166548)
