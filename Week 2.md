
# Day 1: Introduction to Text Representation & Bag of Words

### Topics

* Why text needs numerical representation
* Corpus and vocabulary
* One-hot encoding
* Bag of Words (BoW)
* Document-Term Matrix (DTM)
* Sparse representations
* Limitations of BoW

### Videos

* Stanford NLP: Vector Semantics
* StatQuest: Bag of Words

### Reading

* Jurafsky & Martin, Chapter 6 (Sections 6.1–6.2)

### Practical

* Build vocabulary from a corpus
* Create document-term matrices manually
* Implement BoW using Python dictionaries
* Generate BoW vectors using `CountVectorizer`


---

# Day 2: N-grams and Feature Engineering

### Topics

* Unigrams
* Bigrams
* Trigrams
* Context capture using n-grams
* Vocabulary growth
* Sparsity issues
* Choosing n-gram ranges

### Videos

* Stanford NLP lecture on language modeling
* N-gram tutorial videos

### Reading

* Jurafsky & Martin (N-gram sections)

### Practical

* Generate unigram features
* Generate bigram features
* Compare feature dimensions
* Experiment with different n-gram ranges in sklearn

---

# Day 3: Term Frequency (TF)

### Topics

* Frequency-based representations
* Raw frequency
* Relative frequency
* Importance of term occurrence
* Frequency normalization

### Videos

* TF-IDF intuition videos

### Reading

* Jurafsky & Martin Chapter 6

### Practical

* Compute TF manually
* Implement TF using Python
* Compare TF values across documents

---

# Day 4: Inverse Document Frequency (IDF)

### Topics

* Common vs informative words
* Document Frequency (DF)
* Inverse Document Frequency (IDF)
* Stopwords and their effects
* Rare word importance

### Videos

* StatQuest: TF-IDF (IDF section)

### Reading

* Jurafsky & Martin Chapter 6

### Practical

* Calculate DF manually
* Compute IDF scores
* Identify highly informative terms
---

# Day 5: TF-IDF Representation

### Topics

* TF-IDF intuition
* Combining TF and IDF
* Weighted vector representations
* Advantages over BoW
* Sparse vector representations

### Videos

* StatQuest: TF-IDF

### Reading

* Jurafsky & Martin Chapter 6
* Scikit-Learn TF-IDF documentation

### Practical

* Implement TF-IDF manually
* Use `TfidfVectorizer`
* Compare BoW, TF, and TF-IDF vectors

---

# Day 6: Cosine Similarity and Document Retrieval

### Topics

* Vector similarity
* Dot product
* Euclidean distance
* Cosine similarity
* Similarity-based retrieval
* Ranking documents

### Videos

* StatQuest: Cosine Similarity

### Reading

* Jurafsky & Martin Chapter 6

### Practical

* Implement cosine similarity from scratch
* Use sklearn cosine similarity
* Rank documents based on similarity
---

# Day 7: Mini Project — Document Search Engine

### Topics

* End-to-end retrieval pipeline
* TF-IDF indexing
* Query processing
* Similarity ranking
* Retrieval evaluation

### Practical

Build:

* Document preprocessing pipeline
* TF-IDF index
* Query interface
* Top-k retrieval system

### Dataset Options

* BBC News Dataset
* 20 Newsgroups Dataset
* Custom article collection


---

### Primary References

*  Jurafsky & Martin — Chapter 6: Vector Semantics
*  Scikit-Learn Documentation
*  Stanford NLP Lectures
*  StatQuest (Bag of Words, TF-IDF, Cosine Similarity)

