# Week 1: Introduction to NLP, Text Preprocessing & Simple NLP Pipeline

## Week Objective

- NLP applications and scope
- Text preprocessing pipeline
- Tokenization and normalization
- Morphology basics
- Regex cleaning
- Unicode and UTF-8
- Intro to subword tokenization
- Build preprocessing pipeline

---

Primary Reference https://web.stanford.edu/~jurafsky/slp3/slides/tokens_jan26.pdf / https://web.stanford.edu/~jurafsky/slp3/2.pdf
you can google a video of any topic if you have any doubt otherwise it is very intuitive
also go through https://www.cse.iitb.ac.in/~cs626/2022/Lectures/1-cs626-intro-27jul22.pdf for simple introduction..

## Day 1: NLP Introduction + Words and Corpora

### Topics
- What is NLP
- Applications:
  - Search
  - Translation
  - Chatbots
  - Summarization
  - Sentiment Analysis
  - QA Systems
- NLP vs NLU vs NLG
- Structured vs Unstructured text
- Words vs Tokens
- Types vs Instances
- Vocabulary size |V|
- Token count N
- Corpora
- Function words vs Content words
- Vocabulary growth
- Heaps Law

### Videos
- CS124: Words and Corpora : https://www.youtube.com/watch?v=xsIDTmo1NOg
- NLP Introduction videos 

### Reading
- Jurafsky Ch.2 (Words and Tokens)

---

## Day 2: Tokenization and Text Preprocessing

### Topics
- Lowercasing
- Text normalization
- Tokenization
- Sentence tokenization
- Word tokenization
- Character tokenization
- Subword tokenization
- Tokenization across languages
- Chinese tokenization
- Japanese tokenization issues
- Thai spacing issues
- Unknown words (OOV)

### Practical
- NLTK tokenizer
- spaCy tokenizer

### Videos
- CS124: Word Tokenization: https://www.youtube.com/watch?v=7yFZHf8mzGk&list=PLaZQkZp6WhWyvdiP49JG-rjyTPck_hvEu&index=4

---

## Day 3: Regex and Text Cleaning

### Topics
- Regular expressions
- Regex substitution
- Pattern matching
- Text cleaning
- URL removal
- HTML removal
- Emoji removal
- Numbers removal
- Stopword removal
- Hashtag extraction
- Mention extraction
- Tweet cleaning

### Regex Patterns
- \d
- \w
- \s
- ^
- $
- Emails
- URLs
- Mentions
- Hashtags

### Videos
- CS124: Regular Expressions : https://www.youtube.com/watch?v=808M7q8QX0E&list=PLaZQkZp6WhWyvdiP49JG-rjyTPck_hvEu&index=1
- CS124: Regex Substitutions : https://www.youtube.com/watch?v=1CSVy9JbbK0&list=PLaZQkZp6WhWyvdiP49JG-rjyTPck_hvEu&index=2

---

## Day 4: Morphology and Normalization

### Topics
- Morphemes
- Morphology
- Root morphemes
- Affixes
- Inflectional morphology
- Derivational morphology
- Clitics
- Morphological typology
- Case folding
- Stemming
- Lemmatization
- Porter Stemmer
- Snowball Stemmer
- Lancaster Stemmer
- Word normalization

### Videos
- CS124: Word Normalization : https://www.youtube.com/watch?v=bFfWbQoVmIA&list=PLaZQkZp6WhWyvdiP49JG-rjyTPck_hvEu&index=6

### Reading
- Jurafsky Ch.2 Morphemes

---

## Day 5: Unicode and Encoding

### Topics
- ASCII
- Unicode
- Code points
- UTF-8
- UTF-32
- Character encoding
- Python Unicode handling
- Multilingual text
- CJK characters
- Devanagari scripts
- Emoji encoding

### Reading
- Jurafsky Ch.2 Unicode section

---

## Day 6: Subword Tokenization Preview

### Topics
- Why words fail
- Vocabulary explosion
- OOV words
- Subword tokenization
- Byte Pair Encoding (BPE)
- Token learner
- Token encoder
- Merge operations
- SentencePiece overview
- Intro to LLM tokenizers

### Videos
- CS124: Byte Pair Encoding : https://www.youtube.com/watch?v=tOMjTCO0htA&list=PLaZQkZp6WhWyvdiP49JG-rjyTPck_hvEu&index=5
- other: https://medium.com/@mcraddock/introduction-to-tokenizers-in-large-language-models-llms-using-wardley-maps-652ee4dd6227
---

## Day 7: Mini Project

### Dataset Options
- IMDB Reviews
- Twitter Sentiment
- SMS Spam

### Tasks
1. Load dataset
2. Regex cleaning
3. Lowercase
4. Tokenization
5. Stopword removal
6. Lemmatization
7. Vocabulary analysis
8. Save processed corpus
9. Generate report

### Deliverables
- Notebook
- Clean CSV
- Markdown notes
- Vocabulary statistics

---

## Reading Material

### Primary
- Jurafsky & Martin
  - Chapter 2
    - Words and Tokens
    - Morphemes
    - Unicode
    - Tokenization
    - Normalization
    - BPE

### Supplementary
- NLTK Documentation
- spaCy Documentation
- HuggingFace Tokenizers

