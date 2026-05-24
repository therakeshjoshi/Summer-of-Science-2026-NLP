# Week 1: Introduction to NLP, Text Preprocessing, Words & Tokens, Regex and Simple NLP Pipeline

## Week Objective

By the end of Week 1 you should be able to:

- Understand NLP applications and scope# Week 1: Introduction to NLP, Text Preprocessing & Simple NLP Pipeline

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


- Understand words, tokens, vocabulary and corpora
- Build preprocessing pipelines
- Use regular expressions for cleaning
- Understand morphology and tokenization
- Understand Unicode and UTF‑8
- Perform preprocessing on real datasets
- Gain intuition for future subword tokenization and LLM pipelines

---




Watch these lectures during Week 1:

1. Regular Expressions
2. Regular Expression Substitutions
3. Words and Corpora
4. Word Tokenization
5. Byte Pair Encoding
6. Word Normalization

Suggested sequence:

Day 1:
- Words and Corpora
- NLP Introduction

Day 2:
- Word Tokenization lecture

Day 3:
- Regular Expressions + substitutions

Day 4:
- Word Normalization

Day 5:
- Unicode + Encoding notes

Day 6:
- Byte Pair Encoding overview

Day 7:
- Mini project

Extra practical videos:
- Krish Naik NLP preprocessing playlist
- spaCy tutorials
- NLTK preprocessing tutorials

---

# Day 1: Introduction to NLP + Words and Corpora

## What is NLP?

Natural Language Processing enables machines to:

- Understand language
- Process text
- Generate language
- Extract information

Applications:

1. Search Engines
2. Translation
3. Chatbots
4. Summarization
5. Sentiment Analysis
6. QA Systems
7. Recommendation Systems
8. Speech Recognition

---

## Words vs Tokens

Sentence:

They picnicked by the pool then lay back on the grass and looked at the stars

Concepts:

Type:
Distinct vocabulary item

Token:
Actual occurrence in text

Example:

14 Types

16 Tokens

Study:

- Vocabulary size |V|
- Number of instances N
- Corpus statistics
- Vocabulary growth

Mini task:

Compute:

```python
len(set(tokens))
len(tokens)
```

---

## Word Problems in NLP

Questions:

1. Is "I'm" one word or two?
2. Should punctuation be tokens?
3. Are “They” and “they” same?
4. What about speech fillers?

Example:

uh
um
main-

---

# Day 2: Tokenization and Text Preprocessing

## NLP Pipeline

Raw Text

↓

Cleaning

↓

Normalization

↓

Tokenization

↓

Stopword Removal

↓

Lemmatization

↓

Final Corpus

---

## Tokenization Types

1. Word tokenization
2. Sentence tokenization
3. Character tokenization
4. Subword tokenization

Libraries:

- nltk
- spaCy

Practice:

Implement:

```python
from nltk.tokenize import word_tokenize
from nltk.tokenize import sent_tokenize
```

---

## Tokenization Across Languages

English:

hello world

Chinese:

姚明进入总决赛

Questions:

3 words?

5 words?

7 words?

Discussion:

- Chinese segmentation
- Japanese tokenization
- Thai spacing issues

---

## Too Many Words Problem

Vocabulary grows continuously.

Study:

Heaps Law:

|V| = kN^b

where:

V = vocabulary size

N = corpus size

Reason:

Unknown words always exist.

---

# Day 3: Regex + Text Cleaning

## Regex Basics

Patterns:

Digits:

```python
\d
```

Characters:

```python
\w
```

Whitespace:

```python
\s
```

Beginning:

```python
^
```

End:

```python
$
```

---

## Regex Tasks from Video

Find:

the

Observe:

the

other

there

blithe

Understand substring matching.

---

## Cleaning Tasks

Remove:

- URLs
- HTML
- Emojis
- Numbers
- Extra spaces
- Mentions
- Hashtags

Examples:

Email:

```python
r'[\w\.-]+@[\w\.-]+'
```

URL:

```python
r'https?://\S+'
```

Hashtag:

```python
r'#\w+'
```

Mention:

```python
r'@\w+'
```

Mini Exercise:

Clean tweets dataset.

---

# Day 4: Morphology + Normalization

## Morphemes

Definition:

Smallest meaning unit.

Examples:

fox

1 morpheme

cats

cat + s

worked

work + ed

carefully

care + ful + ly

---

## Types of Morphemes

### Root

Main meaning

Examples:

work

glass

care

### Affixes

Add meaning

-ed

-es

-ly

-ful

---

## Inflectional Morphology

Examples:

worked

past tense

cats

plural

reads

third person

---

## Derivational Morphology

care

↓

careful

↓

carefully

Changes word category.

---

## Clitics

Examples:

I've

teacher's

French l'

Arabic prefixes

---

## Normalization

Case folding:

Woodchuck

↓

woodchuck

Study:

- Lowercasing
- Normalization
- OOV handling
- Lemmatization
- Stemming

---

# Day 5: Unicode and UTF‑8

## Why ASCII was insufficient

Problems:

Spanish:

Señor

Chinese

Hindi

Marathi

Emoji support

---

## Unicode

Unicode:

Universal character representation

Supports:

- 150k+ characters
- Multiple scripts
- Emojis
- Symbols

Code point:

Example:

a

U+0061

---

## UTF‑8 Encoding

ASCII:

1 byte

European languages:

2 bytes

CJK:

3 bytes

Rare symbols:

4 bytes

Advantages:

- Efficient
- Backward compatible
- Self synchronizing

---

## Python Unicode

Study:

```python
len("नमस्ते")
```

Read files:

```python
open(
file,
encoding="utf-8"
)
```

---

# Day 6: Subword Tokenization Preview

Why words fail:

1. No spaces in some languages
2. Vocabulary explosion
3. Unknown words

---

## Byte Pair Encoding

Algorithm:

Repeat:

Find most frequent pair

Merge

Add token

Repeat k times

Example:

A B C A B

↓

AB C AB

↓

CAB

Applications:

- GPT
- BERT tokenizers
- LLM preprocessing

Do NOT master now.

Only intuition.

Detailed study:

Week 3 onwards.

---

# Day 7: Mini Project

Dataset:

Choose one:

- IMDB reviews
- Tweets
- SMS spam

Tasks:

1. Load dataset
2. Regex cleaning
3. Lowercase
4. Tokenization
5. Stopword removal
6. Lemmatization
7. Vocabulary analysis
8. Most frequent words
9. Save cleaned corpus

Deliverables:

- Notebook
- CSV
- Markdown report
- Vocabulary plots

---

# Reading Material

Primary:

Jurafsky and Martin

Speech and Language Processing

Chapter 2

Focus:

- Words
- Tokens
- Morphemes
- Unicode
- Tokenization
- Normalization
- BPE

Supplementary:

1. NLTK docs
2. spaCy docs
3. HuggingFace tokenizer docs
4. CS124 lecture notes

---

