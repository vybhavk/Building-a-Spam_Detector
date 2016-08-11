# Building a Spam detector by using python

To build a model that detects spam mails in given text
The most common ways to extract numerical features from text content, namely: tokenizing strings and giving an integer id for each possible token, for instance by using white-spaces and punctuation as token separators.

 Counting the occurrences of tokens in each document.
 
 Normalizing and weighting with diminishing importance tokens that occur in the majority of samples / documents.

**Step 1 :** First of all we need to clean the text as there will be punctuation, stop words(refer to the most common words in a language) so we have remove all punctuation,remove all stopwords.

**Step 2 :** Create n-grams from the text. we use this by using CountVectorizer module

Tf means term-frequency while tf–idf means term-frequency times inverse document-frequency. This was originally a term weighting scheme developed for information retrieval (as a ranking function for search engines results), that has also found good use in document classification and clustering.

**Step 3:** Normalization is implemented by the TfidfTransformer

MultinomialNB implements the naive Bayes algorithm for multinomially distributed data, and is one of the two classic naive Bayes variants used in text classification (where the data are typically represented as word vector counts, although tf-idf vectors are also known to work well in practice).

**Step 4:** We are using MultinomialNB for building a spam detector 

**Step 5:** Verify the peformance of detector by using classification_report

