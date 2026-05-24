
# Week 1: Introduction to NLP & Text Preprocessing & Simple NLP Pipeline


---

## Day 1: Introduction to NLP

### Topics
#### What is NLP?
Natural Language Processing (NLP) is a branch of AI that enables computers to understand, interpret, process, and generate human language.

### NLP Pipeline Overview
Raw Text → Cleaning → Tokenization → Feature Extraction → Model → Prediction

### Major Applications
1. Search Engines
2. Machine Translation
3. Chatbots and Virtual Assistants
4. Text Summarization
5. Sentiment Analysis
6. Spam Detection
7. Question Answering
8. Information Retrieval
9. Recommendation Systems
10. Speech Systems

### Theory Tasks
- Difference between NLP, NLU and NLG
- Structured vs Unstructured Text
- Challenges:
  - Ambiguity
  - Context dependence
  - Polysemy
  - Sarcasm
  - Domain adaptation

### Practical
Install:
```bash
pip install nltk spacy pandas regex scikit-learn matplotlib
python -m nltk.downloader all
python -m spacy download en_core_web_sm
```

---

## Day 2: Text Preprocessing Pipeline

### Step 1: Lowercasing
Example:
"Machine Learning IS FUN"
→ machine learning is fun

### Step 2: Tokenization
Sentence:
"I love NLP"

Tokens:
["I", "love", "NLP"]

Types:
- Word tokenization
- Sentence tokenization
- Subword tokenization
- Character tokenization

Libraries:
- NLTK
- spaCy

Practice:
Implement both NLTK and spaCy tokenizers.

---

## Day 3: Stopword Removal and Text Cleaning

### Stopwords
Examples:
the, is, am, are, was, in, on

Task:
Remove stopwords and compare outputs.

### Noise Removal
Remove:
- URLs
- HTML tags
- Emojis
- Numbers
- Extra spaces
- Special characters

Example:
Input:
"Great movie!!! Visit https://abc.com :)"

Output:
"great movie"

---

## Day 4: Stemming and Lemmatization

### Stemming
Words:
playing → play
studies → studi

Algorithms:
- Porter Stemmer
- Snowball Stemmer
- Lancaster Stemmer

### Lemmatization
playing → play
better → good

Compare:
| Word | Stem | Lemma |
|------|------|-------|
| running | run | run |
| studies | studi | study |
| better | better | good |

Exercise:
Create comparison table for 50 words.

---

## Day 5: Regular Expressions

### Regex Basics
Patterns:
- Digits: \d
- Characters: \w
- Spaces: \s
- Start: ^
- End: $

Examples:
Emails:
```python
r'[\w\.-]+@[\w\.-]+'
```

URLs:
```python
r'https?://\S+'
```

Hashtags:
```python
r'#\w+'
```

Mentions:
```python
r'@\w+'
```

Mini Tasks:
1. Remove links
2. Extract hashtags
3. Remove emojis
4. Clean tweets

---

## Day 6: Build Simple NLP Pipeline

Pipeline:
1. Raw text input
2. Lowercase
3. Regex cleaning
4. Tokenization
5. Stopword removal
6. Lemmatization
7. Final processed output

Pseudo Code:
```python
text
↓
clean()
↓
tokenize()
↓
remove_stopwords()
↓
lemmatize()
↓
processed_text
```

Dataset Options:
- IMDB Movie Reviews
- Twitter sentiment data
- SMS Spam dataset

---

## Day 7: Mini Project

### Exercise
Clean and preprocess IMDB reviews.

Tasks:
- Load dataset
- Remove noise
- Tokenize
- Remove stopwords
- Lemmatize
- Save processed corpus

Deliverables:
- Jupyter notebook
- Clean CSV
- Documentation

Suggested Evaluation:
- Before vs after cleaning examples
- Vocabulary size reduction
- Most common words

---

## Extra Concepts

Study:
- Unicode handling
- UTF-8 encoding
- OOV words
- Sentence segmentation
- Text normalization
- Case folding

---

## Reading Material

Primary Reading:
Jurafsky & Martin:
Speech and Language Processing
Chapter 2

Supplementary:
1. NLTK Documentation
2. spaCy Documentation
3. Scikit-learn text tutorials

---


