# TF_IDF-with-and-without-use-sklearn---comparing.

First part:

Function (“tfidf_vectorizer”) receive a corpus (list of strings) and the minimal word frequency (words that would occur fewer than this number of times in the corpus will be ignored). FIRST function do not use sklearn algorithms directly. A function returns:

a. Vocab – a dictionary with a mapping of words to ids.

b. Document Frequency: a vector of size len(vocab) containing the number of documents holding the corresponding word. Element i of the vector would contain the number of documents with the word with id i.

c. Word frequency: a vector containing the number of times each word is found in the corpus.

d. Matrix of shape len(documents) x len(vocab) with TF-IDF values for every document in the corpus.

Second Part:

Created a Small search engine, a function called “search” to search for tweets based on
query. The function would receive the data you’ve generated in ‘tfidf_vectorizer’, a list of
tweets to search through, a search query (string) and the number of matches to return.
The function will preprocess the query (same pre-processing as the one you used to
compute tf-idf), convert the query into a vector and find the requested number of the most
similar tweets.
The function will return: a list of tweets ranked by their similarity to the query and a list of
values representing fit of every result.
At the end you will see a few examples of its use. 

Third Part: 

Compare performance of the function you have created in 1) to sklearn
implementation. Which one is faster and by how much? What are the memory requirements
for each? (i.e. how much RAM is consumed to store results for each of the approaches?). 

Fourth part:

The files ‘negative_tweets.txt’ and ‘positive_tweets.txt’ contain negative and positive
tweets correspondingly. I Use WordCloud component (pip install wordcloud) to visualize the
difference between the two corpora (cleaning the tweets before processing them).
I use TF-IDF to support and expand my findings.
