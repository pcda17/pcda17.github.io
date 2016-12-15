# History of "Freedom" and "Democracy"

## Student aim at start of semester:

- Study texts in Project Gutenberg, perhaps searching for changes in political language.

##Week 3: To Do Before Class

>Choose an online data/metadata source, preferably one available to the public via direct download or API. Download a sample of the data, at least 50 or 100 records. Read them over closely, noting anything unexpected. Search for information about the dataset's history, purpose, intended audience, and any past uses by researchers or journalists. Describe what you learned in 400–500 words.

- Read up on Project Gutenberg's limits on automated traffic: https://www.gutenberg.org/wiki/Gutenberg:Information_About_Robot_Access_to_our_Pages
- Download [public Gutenberg metadata](https://www.gutenberg.org/wiki/Gutenberg:Offline_Catalogs) in XML/RDF format and submit sample set of 100 metadata records. 
- Describe how Project Gutenberg uses and extends Dublin Core metadata standard.
```
    <dcterms:issued rdf:datatype="http://www.w3.org/2001/XMLSchema#date">1994-01-01</dcterms:issued>
    <dcterms:creator>
      <pgterms:agent rdf:about="2009/agents/65">
        <pgterms:alias>Shakspeare, William</pgterms:alias>
        <pgterms:alias>Shakspere, William</pgterms:alias>
        <pgterms:birthdate rdf:datatype="http://www.w3.org/2001/XMLSchema#integer">1564</pgterms:birthdate>
        <pgterms:name>Shakespeare, William</pgterms:name>
        <pgterms:deathdate rdf:datatype="http://www.w3.org/2001/XMLSchema#integer">1616</pgterms:deathdate>
        <pgterms:webpage rdf:resource="http://en.wikipedia.org/wiki/William_Shakespeare"/>
      </pgterms:agent>
    </dcterms:creator>
    <dcterms:title>The Complete Works of William Shakespeare</dcterms:title>
    <pgterms:bookshelf>
      <rdf:Description rdf:nodeID="N7ac43d680eb942369cb1eae3990f7828">
        <dcam:memberOf rdf:resource="2009/pgterms/Bookshelf"/>
        <rdf:value>Plays</rdf:value>
      </rdf:Description>
    </pgterms:bookshelf>
```

## Week 4

>Choose a book-length text (or set of texts) available online with which you are familiar. Following Montfort’s code examples, parse the text using the TextBlob library and run some exploratory tests. In 400–500 words, describe your process and what you learned about the text, emphasizing anything you found surprising. Submit your code in a Jupyter notebook.

- Download complete works of two authors included on Project Gutenberg.
- Parse and compare using TextBlob: sentiment analysis, vocabulary size, sentence length, high-frequency terms, etc.

## Week 5

>Choose an API from the list of examples or choose one that is relevant to your final project. An API with a URL-based interface is preferable. Sign up for a developer key if necessary, keeping in mind that it may take a day or two for your request to be processed. Read the documentation for the API and familiarize yourself with it by running a few sample queries. Then execute a larger query (or series of queries) within bounds you choose, aiming to collect at least 2,000–3,000 metadata records. Verify that your dataset is complete and intact. Transform the data to CSV format and conduct any necessary cleaning in Excel, Calc, or OpenRefine. Post 100–200 words on Canvas about your collection process and results.

- Instead of acquiring metadata from an API, which Project Gutenberg doesn't offer, spend this week writing code to parse XML/RDF metadata and export selected fields to CSV format. 
- Define a subset of Project Gutenberg books (e.g., a list of genres or authors) and submit a CSV version of their metadata.

## Week 6: Data and Politics

>In 500–600 words, evaluate the “moral dimension” of the dataset you collected last week. Take the [*list of questions*](https://thefrailestthing.com/2014/11/29/do-artifacts-have-ethics/) posed by Michael Sacasas as a starting point, describing any biases, exclusions, or individual interests reflected in the collection. What can't these data tell you? How might they be used or misused?

- Acquire [collected set](http://www.stephenmclaughlin.net/temp/freedom_democracy/gutenberg2010.zip) of Project Gutenberg ebooks from a third party and align files with existing metadata.
- ​Discuss canons, corpora, and the constructed nature of any "baseline" dataset.

## Week 7: Statistics and Visualization

>Submit a 500–700-word proposal for your final critical data analysis project. What data will you be using? What kind of patterns are you looking for? What critical lens will you apply? Most importantly, who is the intended audience for your study and why would/should they care about your findings? Describe what led you to choose this project and present any preliminary observations and hypotheses. You should consider this assignment an abstract or partial draft toward your final project. Each student should post the proposal two days before class. You will be assigned another student at random, and you will post a 100–200-word response to that student’s proposal before class.

- Final project proposal: Study the words "freedom" and "democracy" as they have been used over time in printed English.
- Refer to the words' [OED entries](http://www.stephenmclaughlin.net/temp/freedom_democracy/freedom_democracy_oed.pdf) and other traditional philological/linguistic resources.
- Describe scope and range of chosen corpus (e.g., works of US and UK nonfiction, 1900–1920).
- Outline experiment: Choose 100 excerpts containing "freedom" and 100 containing "democracy" from texts in a given date range. Evaluate each and apply several codes: Does "democracy" refer to a political system or a political ideal? Does "freedom" refer to individual liberty or to collective welfare?

## Week 8

>Choose an online data/metadata source, preferably the one you’re using for your final project. Using techniques from last week’s readings, present a quantitative exploration of the data using descriptive statistics and two or three visualizations. Up to two of these may be histograms, accompanied by another graphical format of your choice. You may use numerical values included in the collection or quantify some aspect of the data using techniques learned earlier in the course. In 300 words, describe your process and findings. Submit your code in a Jupyter notebook.

- Plot usage rates of "freedom" and "democracy" over all texts in selected corpus, comparing results to [Google Ngam Viewer](https://books.google.com/ngrams/graph?content=freedom%2Cdemocracy&year_start=1800&year_end=2010&corpus=15&smoothing=3&share=&direct_url=t1%3B%2Cfreedom%3B%2Cc0%3B.t1%3B%2Cdemocracy%3B%2Cc0).
- Plot data from hand-coded excerpts over time (likely partial results).

  ​

## Week 9
>Share your complete, cleaned dataset for the final project. In 200 words, describe the collection and the work you’ve done to shape and/or augment it. Submit a sample of your collection and/or processing code in a Jupyter notebook.

- Dataset contents:
  - Cleaned metadata table for full text corpus
  - Cleaned text files for full corpus
  - Collection of ~200 text excerpts with assigned codes


## Week 10
>Choose two machine learning algorithms discussed last week and a set of texts or metadata records, preferably the collection you are using for the final project. In 300–500 words, compare the likely efficacy of the two approaches and discuss how their classifications may differ.

- Discuss potential classification between variations variations in word usage, perhaps correlating with genre/regional/class variations.

## Week 12: Peer Production & Crowdsourcing
>Report your progress toward the final critical data analysis project in 300–500 words. Note your preliminary findings and describe how your perspective and/or approach has changed since you began.

