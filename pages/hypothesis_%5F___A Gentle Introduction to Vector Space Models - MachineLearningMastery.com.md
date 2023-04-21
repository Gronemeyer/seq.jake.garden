hypothesis-uri:: https://machinelearningmastery.com/a-gentle-introduction-to-vector-space-models/
hypothesis-title:: A Gentle Introduction to Vector Space Models - MachineLearningMastery.com
hypothesis-naming-scheme:: 0.2.0

- 📌 Common use of vector space models and cosine distance
  hid:: fxcXIN4eEe2IaTOjW0PT0A
  updated:: 2023-04-18T19:23:27.867863+00:00
  Vector space models are common in information retrieval systems. We can present documents (e.g., a paragraph, a long passage, a book, or even a sentence) as vectors. This vector can be as simple as counting of the words that the document contains (i.e., a bag-of-word model) or a complicated embedding vector (e.g., Doc2Vec). Then a query to find the most relevant document can be answered by ranking all documents by the cosine distance. Cosine distance should be used because we do not want to favor longer or shorter documents, but to focus on what it contains. Hence we leverage the normalization comes with it to consider how relevant are the documents to the query rather than how many times the words on the query are mentioned in a document.
  If we consider each word in a document as a feature and compute the cosine distance, it is the “hard” distance because we do not care about words with similar meanings (e.g. “document” and “passage” have similar meanings but not “distance”). Embedding vectors such as word2vec would allow us to consider the ontology. Computing the cosine distance with the meaning of words considered is the “soft cosine distance“. Libraries such as gensim provides a way to do this.