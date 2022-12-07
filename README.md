# nlp-group-assignment-3

### Explaining the data:
There are 2 files: *doc_keywords_topics* and *topics.* 

**doc_keywords_topics** column definitions
- filename: name of the file from the nltk reuters data
- tag: train/test tag from the nltk reurers data
- text: original, unedited text
- clean_text: data with removed punctuation and escape character tags (e.g. '\t')
- long_text: data WITH punctuation, but words shorter than 4 characters and tagged by nltk.pos_tag as 'NN', 'NNS', 'JJ', 'JJR', or 'JJS'
- keyword_tuples: the output for each document as received from KeyBERT
- keywords: just the list of words from KeyBERT
- keyword_distances: just the list of distances of each keyword from the document (the higher the better)
- topic_*x*: topic of this document, using *x* BERTopic settings
- probs_*x*: list of probs for this doc to be in any of the topics from the BERTopic model
