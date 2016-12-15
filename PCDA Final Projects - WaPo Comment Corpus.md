
# Washington Post Comment Corpus

## Student aim at start of semester:

- Study texts on a national newspaper website.



##Week 3 
>Choose an online data/metadata source, preferably one available to the public via direct download or API. Download a sample of the data, at least 50 or 100 records. Read them over closely, noting anything unexpected. Search for information about the dataset's history, purpose, intended audience, and any past uses by researchers or journalists. Describe what you learned in 400–500 words.

- Use wget to download HTML source for several dozen articles on the Washington Post.
- Describe scope of metadata visible to the public (author, title, newspaper section, etc.).
- Examine HTML to indentify any concealed metadata categories. Note that comments are not included in source downloaded by wget.
- Justify use of Washington Post: politically influential, draws readers from across political spectrum, API available.


## Week 4

>Choose a book-length text (or set of texts) available online with which you are familiar. Following Montfort’s code examples, parse the text using the TextBlob library and run some exploratory tests. In 400–500 words, describe your process and what you learned about the text, emphasizing anything you found surprising. Submit your code in a Jupyter notebook.

- Use [newspaper](https://pypi.python.org/pypi/newspaper) Python module to download plain text versions of 40 Washington Post articles from four sections: Politics, Business, Opinions, Sports.
- Compare four groups with the aid of tools in TextBlob: sentiment analysis, vocabulary size, sentence length, high-frequency terms, etc.


## Week 5

>Choose an API from the list of examples or choose one that is relevant to your final project. An API with a URL-based interface is preferable. Sign up for a developer key if necessary, keeping in mind that it may take a day or two for your request to be processed. Read the documentation for the API and familiarize yourself with it by running a few sample queries. Then execute a larger query (or series of queries) within bounds you choose, aiming to collect at least 2,000–3,000 metadata records. Verify that your dataset is complete and intact. Transform the data to CSV format and conduct any necessary cleaning in Excel, Calc, or OpenRefine. Post 100–200 words on Canvas about your collection process and results.

- Acquire API key for [The Washington Post API](https://newsapi.org/the-washington-post-api), which returns JSON-formatted metadata:


```
{
"author": "James McAuley",
"title": "Marine Le Pen could win the French election — but first she must win a family feud",
"description": "The far-right dynastic clan is locked in a generational dispute over what direction to take.",
"url": "https://www.washingtonpost.com/world/europe/marine-le-pen-could-win-the-french-election----but-first-she-has-to-win-the-le-pen-family-feud/2016/12/13/dfb46059-bbc3-4f79-a88e-7a23cf0831a5_story.html",
"urlToImage": "https://img.washingtonpost.com/rf/image_1484w/2010-2019/WashingtonPost/2016/12/12/Interactivity/Images/RTR4G3X9.JPG",
"publishedAt": "2016-12-14T10:00:00Z"
}
```

- Download metadata for 2,000 most recent articles, or perhaps assemble thematic article groups based on keyword searches.
- Convert JSON data to CSV, creating master metadata table. Note any inconsistencies/missing values.

## Week 6: Data and Politics

>In 500–600 words, evaluate the “moral dimension” of the dataset you collected last week. Take the [*list of questions*](https://thefrailestthing.com/2014/11/29/do-artifacts-have-ethics/) posed by Michael Sacasas as a starting point, describing any biases, exclusions, or individual interests reflected in the collection. What can't these data tell you? How might they be used or misused?

- Shift project focus to the comment streams beneath articles, which hold the promise of civil discourse yet are often overwhelmed with partisan mockery and trolling. 



## Week 7: Statistics and Visualization

>Submit a 500–700-word proposal for your final critical data analysis project. What data will you be using? What kind of patterns are you looking for? What critical lens will you apply? Most importantly, who is the intended audience for your study and why would/should they care about your findings? Describe what led you to choose this project and present any preliminary observations and hypotheses. You should consider this assignment an abstract or partial draft toward your final project. Each student should post the proposal two days before class. You will be assigned another student at random, and you will post a 100–200-word response to that student’s proposal before class.

- Final project proposal: An analysis of comment streams for 10 recent articles in the Washington Post "Politics" section, with articles chosen at random over a single week.
- Data collection will involve accessing URLs in metadata collected from API. Because Washington Post comments are displayed using JavaScript, pages must first be rendered using PhantomJS, e.g., via the Python package Selenium.
- 250 comments will be hand-classified by political orientation (if apparent within the comment).


## Week 8: Machine Learning

>Choose an online data/metadata source, preferably the one you’re using for your final project. Using techniques from last week’s readings, present a quantitative exploration of the data using descriptive statistics and two or three visualizations. Up to two of these may be histograms, accompanied by another graphical format of your choice. You may use numerical values included in the collection or quantify some aspect of the data using techniques learned earlier in the course. In 300 words, describe your process and findings. Submit your code in a Jupyter notebook.

- Plot comment rates over time after articles are posted. Compare plots for popular and less popular articles.
- Create pie chart of comments classified by political orientation (work likely ongoing).
- Meanwhile, continue cleaning data (e.g., improving parsing of Javascript-generated comment code).



## Week 9
>Share your complete, cleaned dataset for the final project. In 200 words, describe the collection and the work you’ve done to shape and/or augment it. Submit a sample of your collection and/or processing code in a Jupyter notebook.

- Final dataset:
  - CSV table containing 250 hand-coded comments with assigned sentiment values.
  - CSV tables or JSON files containing ~6000 collected comments, along with associated metadata.

## Week 10

>Choose two machine learning algorithms discussed last week and a set of texts or metadata records, preferably the collection you are using for the final project. In 300–500 words, compare the likely efficacy of the two approaches and discuss how their classifications may differ.

- Train a Naive Bayes classifier using comments in liberal and conservative categories. Identify vocabulary cues that may be leading the classifier to succeed/fail.

## Week 12
>Report your progress toward the final critical data analysis project in 300–500 words. Note your preliminary findings and describe how your perspective and/or approach has changed since you began.

- Do sentiment analysis measures correspond with differences in apparent political orientation?
- Which political orientation (if either) appears more likely to provoke conflict?
- In reading the corpus closely, do we see any evidence of changes in opinion?



