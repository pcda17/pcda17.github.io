## Week 5: Word-Level Text Analysis



## *> Review Exercises*

```
sample_text = "A foolish consistency is the hobgoblin of little minds, adored by little statesmen and philosophers and divines. With consistency a great soul has simply nothing to do. He may as well concern himself with his shadow on the wall. Speak what you think now in hard words, and to-morrow speak what to-morrow thinks in hard words again, though it contradict every thing you said to-day. — 'Ah, so you shall be sure to be misunderstood.' — Is it so bad, then, to be misunderstood? Pythagoras was misunderstood, and Socrates, and Jesus, and Luther, and Copernicus, and Galileo, and Newton, and every pure and wise spirit that ever took flesh. To be great is to be misunderstood."

print(sample_text)
```


Split the sample text above into a list of words. Don't worry about punctuation and other oddities.

```
sample_text_words = sample_text.split()

print(sample_text_words)
```



Create a function that takes a text string as an argument and returns the number of words in the text.

```
def word_count(text):
    return len(sample_text.split(' '))

print(word_count(sample_text))
```


Create a list that contains the first letter of each word in the sample text.
> Hint: Use the `append()` function to add items to your list.

```
first_letters = []

for word in sample_text.split(' '):
    first_letters.append(word[0])

print(first_letters)
```


Create a list that contains the length, in characters, of each word in the sample text.

```
word_lengths = []

for word in sample_text.split(' '):
    word_lengths.append(len(word))

print(word_lengths)
```


Create a function that takes a text string as an argument and returns the average word length in the text.


```
import numpy as np

def average_word_length(text):
    word_lengths = []
    for word in sample_text.split(' '):
        word_lengths.append(len(word))
    return np.mean(word_lengths)

print(average_word_length(sample_text))
```


## *> Quick Exercise*

Create a function that returns the top 20 most frequent words in a given TextBlob object. Hint: Use the itemgetter module to sort a list of lists by a given index.


# A possible solution:

```
from operator import itemgetter
from pprint import pprint

freq_dict = text1.word_counts
freq_list = []

for key in freq_dict:
    freq_list.append([key, freq_dict[key]])

sorted_freq_list = sorted(freq_list, key=itemgetter(1))[::-1]

pprint(sorted_freq_list[:30])
```


------------------------------------------



------------------------------------------



------------------------------------------





## *> Quick Exercise*

Referencing the code above, create a function that returns a sorted list of stopword-free word frequency lists when passed a TextBlob object. Look at the top vocabulary for several texts by each of your authors. How similar or different are these frequency lists between texts and between authors?



# A possible solution:

```
def topwords(blob):
    stopwords_eng = stopwords.words('english')
    freq_dict=blob.word_counts
    freq_sans_stopwords = []
    for key in freq_dict:
        lemma = Word(key).lemmatize()
        if lemma not in stopwords_eng:
            freq_sans_stopwords.append([key, freq_dict[key]])
    sorted_freq_sans_stopwords = sorted(freq_sans_stopwords, key = itemgetter(1))[::-1]
    return sorted_freq_sans_stopwords

pprint(topwords(text1)[:20])
print()
pprint(topwords(text2)[:20])
```







------------------------------------------



------------------------------------------



------------------------------------------






## *> Exercise*

Create a function called `POS_profile` that takes a TextBlob object and returns a list containing several parts of speech and their relative frequency within the text. Your POS profile should include the following parts of speech:

- nouns
- adjectives
- verbs
- adverbs
- pronouns

You can find a full list of POS tags used by TextBlob [here](https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html). Note that several parts of speech are split into multiple codes (e.g., NN, NNS, NNP, and NNPS for different classes of noun).

Next, run your POS profile on each text in your two corpora. How much do these values vary between authors and among texts by the same author?



# A possible solution:

```
def POS_profile(blob):
    noun_codes=['NN','NNS','NNP','NNPS']
    adj_codes=['JJ','JJR','JJS']
    verb_codes=['VB','VBD','VBG','VBN','VBP','VBZ']
    adv_codes=['RB','RBR','RBS']
    pronoun_codes=['PRP']
    noun_count=0
    adj_count=0
    verb_count=0
    adv_count=0
    pronoun_count=0
    for (word, tag) in blob.tags:
        if tag in noun_codes: noun_count+=1
        if tag in adj_codes: adj_count+=1
        if tag in verb_codes: verb_count+=1
        if tag in adv_codes: adv_count+=1
        if tag in pronoun_codes: pronoun_count+=1
    word_count=len(blob.words)
    return [float(noun_count)/word_count, float(adj_count)/word_count, float(verb_count)/word_count, float(adv_count)/word_count, float(pronoun_count)/word_count]
```
