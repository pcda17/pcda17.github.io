
# Syllabus: Programming for Cultural Data Analysis

#### University of Texas at Austin School of Information

Fall 2017, Mondays 3–6 p.m.

Instructor: Tanya Clement

TA: Steve McLaughlin

Office hours: Mondays 1–3 p.m., UTA 5.558


##### Course Schedule

[Week 1](#week1) | [Week 2](#week2) | [Week 3](#week3) | [Week 4](#week4) | 
[Week 5](#week5) | [Week 6](#week6) | [Week 7](#week7) | [Week 8](#week8) | 
[Week 9](#week9) | [Week 10](#week10) | [Week 11](#week11) | [Week 12](#week12)
 | [Week 13](#week13) | [Week 14](#week14)

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

<!--
### Resources

-   Software Tools

-   Sample Data Sources
-->



----------------------------------------------------------------


# <a name="week1"></a>Week 1 (9/11): Introductions & Command Line Basics

### Readings

**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_1)**

-   Nick Montfort (2016) “Why Program?” In *Exploratory Programming for the Arts and Humanities*, 267–77. Cambridge, MA: The MIT Press.

-   danah boyd & Kate Crawford (2012) "Critical Questions for Big Data," *Information, Communication & Society*, 15:5, 662-679.

To start for next week:
-   Neal Stephenson (1999) “In the Beginning Was the Command Line.” Cryptonomicon. [Note: This reading is due the second week of the course but it's quite long.] <http://www.cryptonomicon.com/beginning.html>. [TXT](http://www.cryptonomicon.com/command.zip).


##### [▸ In-class outline](week-01.md)



----------------------------------------------------------------



# <a name="week2"></a>Week 2 (9/18): The Operating System in Context


### Readings

**[Readings in Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_2)**

-   Noria, Xavier. “Understanding Newlines.” *O’Reilly ONLamp*, August 17, 2006. [http://www.onlamp.com/pub/a/onlamp/2006/08/17/understanding-newlines.html](http://www.onlamp.com/pub/a/onlamp/2006/08/17/understanding-newlines.html)

-   Oualline, Steve. “The End of Line Puzzle.” *The Practical Programmer*. [http://www.oualline.com/practical.programmer/eol.html](http://www.oualline.com/practical.programmer/eol.html)

-   Piper, Andrew. "There will be Numbers." *Journal of Cultural Analytics* 1, no. 1 (May 23, 2016). [http://culturalanalytics.org/2016/05/there-will-be-numbers/](http://culturalanalytics.org/2016/05/there-will-be-numbers/)

-   Stephenson, Neal. “In the Beginning Was the Command Line.” Cryptonomicon, 1999. <http://www.cryptonomicon.com/beginning.html>. [TXT](http://www.cryptonomicon.com/command.zip). 

### Optional
Read pages 1–28 of Shieber’s Python tutorial and work through the code examples.

-   Shieber, Stuart M., *Programming for Humanists* pages 1–28, 2014. [http://blogs.harvard.edu/programmingforhumanists/files/2014/12/proghum.pdf](http://blogs.harvard.edu/programmingforhumanists/files/2014/12/proghum.pdf)

Work through Chris Albon’s tutorial on Python string operations.
-   Albon, Chris. “String Operations.” [http://chrisalbon.com/python/string_operations.html](http://chrisalbon.com/python/string_operations.html)

-   Neff, Gina, Tanweer, Anissa, Fiore-Gartland, Brittany, Osburn, Laura  Critique and Contribute: A Practice-Based Framework for Improving Critical Data Studies and Data Science. *Big Data* 5, no. 2, 2017.


### Assignment


[WA #1](https://utexas.instructure.com/courses/1204381/discussion_topics/2826310)


##### [▸ In-class outline](week-02.md)




----------------------------------------------------------------

# <a name="week3"></a>Week 3 (9/25): Collections as Data: Meaning making

### Readings
**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_3)**

- “The Jupyter Notebook.” [http://jupyter-notebook.readthedocs.io/en/latest/notebook.html](http://jupyter-notebook.readthedocs.io/en/latest/notebook.html)

<!--move the below to week 2-->
- Allardice, Simon. “Foundations of Programming: Fundamentals, parts 1-3; part 5, just "part 5, Breaking your code apart"; and part 14, just “Python” and “Libraries and frameworks”. [http://www.lynda.com/JavaScript-tutorials/Foundations-of-Programming-Fundamentals/83603-2.html](http://www.lynda.com/JavaScript-tutorials/Foundations-of-Programming-Fundamentals/83603-2.html) [To access Lynda.com. follow links below, click “Log in,” then “Organizational Login,” and enter your UT EID and password.]

- Clement, T. and McLaughlin, S. “Measured Applause: Toward a Cultural Analysis of Audio Collections.” Cultural Analytics, vol. 1, no. 1, 2016. [http://culturalanalytics.org/2016/05/measured-applause-toward-a-cultural-analysis-of-audio-collections/](http://culturalanalytics.org/2016/05/measured-applause-toward-a-cultural-analysis-of-audio-collections/)

- Introna, L. D. “The Enframing of Code: Agency, Originality and the Plagiarist.” *Theory, Culture & Society* 28, no. 6 (November 1, 2011): 113–41.

- Liu, Alan. “The Meaning of the Digital Humanities.” *PMLA* 128, no. 2 (March 2013): 409–23.

- Padilla, T. "On a Collections as Data Imperative." [PDF](http://digitalpreservation.gov/meetings/dcs16/tpadilla_OnaCollectionsasDataImperative_final.pdf).


### Optional

-  Gallinger, M. and Daniel Chudnov "Library of Congress Lab: Library of Congress Digital Scholars Lab Pilot Project Report."
-  Posner, Miriam. “Humanities Data: A Necessary Contradiction.” *Miriam Posner’s Blog*, June 25, 2015. [http://miriamposner.com/blog/humanities-data-a-necessary-contradiction](http://miriamposner.com/blog/humanities-data-a-necessary-contradiction)

-  Marini, Joe. “Up and Running with Python.” Lynda.com.
            [http://www.lynda.com/Python-tutorials/Welcome/122467/142550-4.html](http://www.lynda.com/Python-tutorials/Welcome/122467/142550-4.html)


### Assignment

[WA #2](https://utexas.instructure.com/courses/1204381/discussion_topics/2840058)


##### [▸ In-class outline](week-03.md)



----------------------------------------------------------------

# <a name="week4"></a>Week 4 (10/2): Collections as Data: Data Models

### Readings

**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_4)**

-   Albon, Chris. “Parse JSON File.” [http://chrisalbon.com/python/json_parse_file.html](http://chrisalbon.com/python/json_parse_file.html)

-   Fortune, Stephen. “A Brief History of Databases.” *Avant*, February 27th 2014. [https://web.archive.org/web/20150220031213/http://avant.org/media/history-of-databases](https://web.archive.org/web/20150220031213/http://avant.org/media/history-of-databases)

-   van Hooland, Seth, and Ruben Verborgh. “Modelling.” In *Linked Data for Libraries, Archives and Museums: How to Clean, Link and Publish Your Metadata*, 11–70. Chicago: Neal-Schuman, 2014.

-   Zhuang, Atima Han, Ishita Vedvyas, and Rishikesh Dole. “Tutorial: OpenRefine,” 2013. [http://casci.umd.edu/wp-content/uploads/2013/12/OpenRefine-tutorial-v1.5.pdf](http://casci.umd.edu/wp-content/uploads/2013/12/OpenRefine-tutorial-v1.5.pdf)


### Optional Readings

-   Lundh, Fredrik. “Elements and Element Trees.” [http://effbot.org/zone/element.htm](http://effbot.org/zone/element.htm) [Python XML tutorial]

-   Beazley, David, and Brian K. Jones. “Chapter 6: Data Encoding and Processing.” In Python Cookbook: *recipes for Mastering Python 3*, 3. ed., 175–216. Bejing: O’Reilly, 2013.

### Assignment

[WA #3](https://utexas.instructure.com/courses/1204381/discussion_topics/2841839)

##### [▸ In-class outline](week-04.md)



----------------------------------------------------------------



# <a name="week5"></a>Week 5 (10/9): Word-Level Text Analysis


<! -- Install textblob package before class (a wrapper for NLTK and pattern) and work through Montfort’s code examples. The --user option lets us install a module for the current user only, without requiring an admin password.

pip install --user -U textblob

python -m textblob.download_corpora
-->


### Readings

**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_5)**

-   Burrows, John. “Textual Analysis.” In *Companion to Digital Humanities*, edited by Susan Schreibman, Ray Siemens, and John Unsworth. [Link](http://digitalhumanities.org/companion/view?docId=blackwell/9781405103213/9781405103213.xml&doc.view=print&chunk.id=ss1-4-4&toc.depth=1&toc.id=0).

-   Ramsay, Stephen. “Chapter 1: An Algorithmic Criticism.” In *Reading Machines: Toward an Algorithmic Criticism*, 1–17. Topics in the Digital Humanities. Urbana: University of Illinois Press, 2011.

-   Montfort, Nick. “Text III.” In *Exploratory Programming for the Arts and Humanities*, 185–213. Cambridge, MA: The MIT Press, 2016. 

-   Fellenbaum, Christiane. “Wordnet(s).” In The *Encyclopedia of Language & Linguistics*, edited by E. K. Brown and Anne Anderson, 2nd ed., 14:665–79. Amsterdam ; Boston: Elsevier, 2005. 

-   “Alphabetical list of part-of-speech tags used in the Penn Treebank Project.” [https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html](https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html)


### Assignment


[WA #4](https://utexas.instructure.com/courses/1204381/discussion_topics/2841813)

##### [▸ In-class outline](week-05.md)



----------------------------------------------------------------


# <a name="week6"></a>Week 6 (10/16): Web Scraping & APIs

Install [Beauitful Soup](https://www.crummy.com/software/BeautifulSoup/) library for parsing HTML.

> pip install -U --user beautifulsoup

Work through Chris Albon’s Beautiful Soup tutorial.

### Readings

**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_6)**

-   Pomerantz, Jeffrey. “The Future of Metadata.” In *Metadata*. The MIT Press Essential Knowledge Series. Cambridge, MA ; London, England: The MIT Press, 2015. 

-   Swartz, Aaron. “Building a Platform: Providing APIs.” In *Aaron Swartz’s ‘A Programmable Web’: An Unfinished Work*, 31–39. San Rafael, CA: Morgan & Claypool Publishers, 2013. 

-   Kelly, Chelsea Emelie. “Beyond Digital: Open Collections & Cultural Institutions,” 2014. *https://artmuseumteaching.com/2014/11/06/beyond-digital-open-collections-cultural-institutions*

-   “HTML Introduction” and “HTML5 Introduction.” W3Schools.

    -   [http://www.w3schools.com/html/html_intro.asp](http://www.w3schools.com/html/html_intro.asp)

    -   [http://www.w3schools.com/html/html5_intro.asp](http://www.w3schools.com/html/html5_intro.asp)

-   Albon, Chris. “Beautiful Soup Basic HTML Scraping.” [http://chrisalbon.com/python/beautiful_soup_html_basics.html](http://chrisalbon.com/python/beautiful_soup_html_basics.html)


### Optional Readings

-   Sanger, David E., and Eric Schmitt. “Snowden Used Low-Cost Tool to Best N.S.A.” The New York Times. February 8, 2014. [http://www.nytimes.com/2014/02/09/us/snowden-used-low-cost-tool-to-best-nsa.html](http://www.nytimes.com/2014/02/09/us/snowden-used-low-cost-tool-to-best-nsa.html)

-   Kazil, Jacqueline, and Katharine Jarmul. “PDFs and Problem Solving in Python.” In *Data Wrangling with Python: Tips and Tools to Make Your Life Easier*, 91–126. O’Reilly, 2016. 

### Assignment

[WA #5](https://utexas.instructure.com/courses/1204381/discussion_topics/2841854)

##### [▸ In-class outline](week-06.md)



----------------------------------------------------------------


# <a name="week7"></a>Week 7 (10/23) The Politics of Data

### Readings

**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_7)**

-  Christen, Kim. “Does Information Really Want to be Free? Indigenous Knowledge Systems and the Question of Openness.” International Journal of Communication 6 (2012), 2870–2893.

-   Peters, Justin. *The Idealist: Aaron Swartz and the Rise of Free Culture on the Internet*, Chapters 7 and 8. New York: Scribner, 2016. 

-   Greenwald, Glenn. “Chapter 1: Contact.” In *No Place to Hide: Edward Snowden, the NSA, and the U.S. Surveillance State*, 2015. 

-   Freelon, Deen Goodwin, Charlton D. McIlwain, and Meredith D. Clark. “Beyond the Hashtags: #Ferguson, #Blacklivesmatter, and the Online Struggle for Offline Justice,” 2016. [http://cmsimpact.org/wp-content/uploads/2016/03/beyond_the_hashtags_2016.pdf](http://cmsimpact.org/wp-content/uploads/2016/03/beyond_the_hashtags_2016.pdf)

-   American Civil Liberties Union. "First Amendment Lawsuit Brought on Behalf of Academic Researchers and Journalists Who Fear Prosecution Under the Computer Fraud and Abuse Act." [https://www.aclu.org/news/aclu-challenges-law-preventing-studies-big-data-discrimination](https://www.aclu.org/news/aclu-challenges-law-preventing-studies-big-data-discrimination)

### Optional Readings

-   Day, Ronald E. “Governing Expression: Social Big Data and Neoliberalism.” In *Indexing It All: The Subject in the Age of Documentation*, Information, and Data, 123–44. History and Foundations of Information Science. Cambridge, Massachusetts: The MIT Press, 2014. 

-   Hitchcock, Tim. “Digital Searching and the Re-formulation of Historical Knowledge” 2008. In *The Virtual Representation of the Past*, edited by Mark Greenglass and Lorna Hughes, 81-90. Ashgate: 2008. 

### Assignment

[WA #6](https://utexas.instructure.com/courses/1204381/discussion_topics/2841926)

##### [▸ In-class outline](week-07.md)



----------------------------------------------------------------


# <a name="week8"></a>Week 8 (10/30): Your Data, Your culture

### Readings

**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_8)**

-   Winner, Langdon. “Do Artifacts Have Politics?” *Daedalus* 109, no. 1 (1980): 121–36. 

-   Joerges, B. “Do Politics Have Artefacts?” *Social Studies of Science* 29, no. 3 (June 1, 1999): 411–31. 

-   Sacasas, Michael. “Do Artifacts Have Ethics?” *The Frailest Thing*, November 29, 2014. [http://thefrailestthing.com/2014/11/29/do-artifacts-have-ethics](http://thefrailestthing.com/2014/11/29/do-artifacts-have-ethics/)


### Assignment

[Due: Proposal](https://utexas.instructure.com/courses/1204381/assignments/4166696)


##### [▸ In-class outline](week-08.md)



----------------------------------------------------------------


# <a name="week9"></a>Week 9 (11/6): Statistics and Visualization


Install [numpy](http://www.numpy.org/) scientific computing library for Python.

> pip install --user -U numpy

Install [pandas](http://pandas.pydata.org/) data analysis library for Python.

> pip install --user -U pandas

Install [matplotlib](http://matplotlib.org/) visualization library for Python.

> pip install --user -U matplotlib

### Readings


**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_9)**

-   Montfort, Nick. Excerpt from “Statistics and Visualization.” In *Exploratory Programming for the Arts and Humanities*, 215–40. Cambridge, MA: The MIT Press, 2016. 

-   Krumme, Coco. “What Data Doesn’t Do.” In *Beautiful Data: The Stories behind Elegant Data Solutions*, edited by Toby Segaran and Jeff Hammerbacher, 1st ed. Beijing ; Sebastopol, CA: O’Reilly, 2009. 

-   Manovich, Lev. “What Is Visualisation?” *Visual Studies* 26, no. 1 (March 15, 2011): 36–49. *http://www.tandfonline.com/doi/abs/10.1080/1472586X.2011.548488*. 

-   Moretti, Franco. “Graphs.” In *Graphs, Maps, Trees: Abstract Models for Literary History*, 3–33. London ; New York: Verso, 2007. 

-   McCandles, David. *Information is Beautiful*. *http://www.informationisbeautiful.net*


### Optional Readings

-   Gries, Stefan. “Useful statistics for corpus linguistics.” <http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.160.9846&rep=rep1&type=pdf>

-   Thompson, Clive. “The Surprising History of the Infographic.” <http://www.smithsonianmag.com/history/surprising-history-infographic-180959563/?no-ist>

### Assignment

[Due: Proposal Peer Review](https://utexas.instructure.com/courses/1204381/assignments/4166696).


##### [▸ In-class outline](week-09.md)



----------------------------------------------------------------


# <a name="week10"></a>Week 10 (11/13): Machine Learning

### Readings

**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_10)**

-   Berendt, Bettina, Preibusch, Soren. Toward Accountable Discrimination-Aware Data Mining:The Importance of Keeping the Human in the Loop—and Under the Looking Glass.Big DataVolume 5, Number 2, 2017.

-   Brew, Chris. “Language Processing: Statistical Methods.” In Encyclopedia of Language & Linguistics, edited by Keith Brown, 2nd ed., 12:597–604. Elsevier, 2006. 

-   Julia Angwin, Jeff Larson, Surya Mattu and Lauren Kirchner, ProPublica. “Machine Bias.” *ProPublica*. May 23, 2016. [https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)

-   “Working With Text Data.” scikit-learn.
                      [http://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html](http://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html)

-   Geitgey, Adam. “Machine Learning is Fun!” *Medium*. [https://medium.com/@ageitgey/machine-learning-is-fun-80ea3ec3c471](https://medium.com/@ageitgey/machine-learning-is-fun-80ea3ec3c471)



### Optional Readings

-   Norvig, Peter. “Natural Language Corpus Data.” In *Beautiful Data: The Stories Behind Elegant Data Solutions*, edited by Toby Segaran and Jeff Hammerbacher, 1st ed. Beijing ; Sebastopol, CA: O’Reilly, 2009. 

-   Baharudin, Baharum, Lam Hong Lee, and Khairullah Khan. “A Review of Machine Learning Algorithms for Text-Documents Classification.” *Journal of Advances in Information Technology* 1, no. 1 (February 1, 2010). 

-   Wolfram, S. Machine Learning for Middle Schoolers. Stephen Wolfram Blog. 11 May 2017. [http://blog.stephenwolfram.com/2017/05/machine-learning-for-middle-schoolers/#comments](http://blog.stephenwolfram.com/2017/05/machine-learning-for-middle-schoolers/#comments) 

### Assignment

[WA #7](https://utexas.instructure.com/courses/1204381/discussion_topics/2842235)

##### [▸ In-class outline](week-10.md)



----------------------------------------------------------------


# <a name="week11"></a>Week 11 (11/20): Critical Text Analysis

### Readings


**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_11)**


-   Hall, Gary. “Toward a Postdigital Humanities: Cultural Analytics and the Computational Turn to Data-Driven Scholarship.” *American Literature* 85, no. 4 (January 1, 2013): 781–809. 

-   Jockers, Matthew Lee. “Chapter 8: Theme.” In *Macroanalysis: Digital Methods and Literary History*, 118–53. Topics in the Digital Humanities. Urbana: University of Illinois Press, 2013. 

-   Marche, Stephen. “Literature Is not Data: Against Digital Humanities.” *Los Angeles Review of Books*, October 28th, 2012.
                      [https://lareviewofbooks.org/essay/literature-is-not-data-against-digital-humanities](https://lareviewofbooks.org/essay/literature-is-not-data-against-digital-humanities)

### Optional Reading

-   Ramsay, Stephen. “Chapter 3: Potential Readings.” In *Reading Machines: Toward an Algorithmic Criticism*, 33–57. Topics in the Digital Humanities. Urbana: University of Illinois Press, 2011. 


### Assignment

[WA #8](https://utexas.instructure.com/courses/1204381/discussion_topics/2842240)


##### [▸ In-class outline](week-11.md)


----------------------------------------------------------------


# <a name="week12"></a>Week 12 (11/27): Copyright and the Information Commons

### Readings

**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_12)**

-   Sims, Nancy. “Library Licensing and Criminal Law: The Aaron Swartz Case.” *College & Research Libraries News* 72, no. 9 (2011): 534–37. [http://crln.acrl.org/content/72/9/534.short](http://crln.acrl.org/content/72/9/534.short).

-   O’Sullivan, Michael. “Aaron Swartz, New Technologies, and the Myth of Open Access.” In *Academic Barbarism, Universities and Inequality*. Palgrave Critical University Studies. Houndmills, Basingstoke, Hampshire ; New York, NY: Palgrave Macmillan, 2016. 

-   “The Digital Public Library of America Policy Statement on Metadata,” 2013. [http://dp.la/info/wp-content/uploads/2013/04/DPLAMetadataPolicy.pdf](http://dp.la/info/wp-content/uploads/2013/04/DPLAMetadataPolicy.pdf)

-   “Creative Commons: About the Licenses.” [https://creativecommons.org/licenses/](https://creativecommons.org/licenses/)

-   DRM article: [http://infojustice.org/wp-content/uploads/2015/03/band03102015.pdf](http://infojustice.org/wp-content/uploads/2015/03/band03102015.pdf)


### Optional Readings

-   Code of Best Practices in Fair Use for Academic and Research Libraries*. Association of Research Libraries, 2012*. [http://www.arl.org/storage/documents/publications/code-of-best-practices-fair-use.pdf](http://www.arl.org/storage/documents/publications/code-of-best-practices-fair-use.pdf)


### Assignment

[WA #9](https://utexas.instructure.com/courses/1204381/discussion_topics/2842243)


##### [▸ In-class outline](week-12.md)



----------------------------------------------------------------


# <a name="week13"></a>Week 13 (12/4): Peer Production & Crowdsourcing

### Readings

**[Canvas](https://utexas.instructure.com/courses/1204381/files/folder/Week_13)**

-   Benkler, Yochai. “Peer Production and Sharing.” In *The Wealth of Networks: How Social Production Transforms Markets and Freedom*, 59–90. New Haven [Conn.]: Yale University Press, 2006.

-   Manzo, Christina, Geoff Kaufman, Sukdith Punjasthitkul, and Mary Flanagan. “‘By the People, For the People’: Assessing the Value of Crowdsourced, User-Generated Metadata.” *Digital Humanities Quarterly* 9, no. 1 (2015). [http://www.digitalhumanities.org/dhq/vol/9/1/000204/000204.html](http://www.digitalhumanities.org/dhq/vol/9/1/000204/000204.html)

-   Bodó, Balázs. “Set the Fox to Watch the Geese: Voluntary IP Regimes in Piratical File-sharing Communities.” In Piracy: Leakages from Modernity, edited by James Arvanitakis and Martin Fredriksson, 241–63. Sacramento, CA: Litwin Books, 2014. 

### Optional Readings

-   Benkler, Yochai, and Helen Nissenbaum. “Commons-Based Peer Production and Virtue.” Journal of Political Philosophy 14, no. 4 (2006): 394–419. [https://www.nyu.edu/projects/nissenbaum/papers/jopp_235.pdf](https://www.nyu.edu/projects/nissenbaum/papers/jopp_235.pdf).

-   Kreiss, D., M. Finn, and F. Turner. “The Limits of Peer Production: Some Reminders from Max Weber for the Network Society.” New Media & Society 13, no. 2 (March 1, 2011): 243–59. 


### Assignment

[WA #10]()

##### [▸ In-class outline](week-13.md)


----------------------------------------------------------------

# <a name="week14"></a>Week 14 (12/11): Final Presentations

[Final Presentation due](https://utexas.instructure.com/courses/1204381/assignments/4166564)

-- **[Installation Tutorials](tutorials/)**

12/18: [Final Project due](https://utexas.instructure.com/courses/1204381/assignments/4166548)
