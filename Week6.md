# Week 6: Attention Mechanism and Sequence-to-Sequence Models

## Week Objective

- Understand the limitations of RNNs and LSTMs
- Learn the Encoder-Decoder (Seq2Seq) architecture
- Understand the Attention Mechanism
- Study different attention variants
- Implement Seq2Seq models using PyTorch
- Apply attention-based models to machine translation and text generation

---

# Day 1 (Monday): Introduction to Sequence-to-Sequence Learning

## Topics
- Review of RNNs and LSTMs
- Limitations of Fixed-Length Context Vectors
- Motivation for Seq2Seq Models
- Encoder-Decoder Architecture
- Sequence-to-Sequence Learning
- Training vs Inference
- Teacher Forcing

## Mathematical Concepts
- Encoder hidden representation
- Decoder hidden representation
- Context vector

## Practical
- Visualize Encoder-Decoder architecture
- Implement a simple Seq2Seq model without attention

## Reading
- Sutskever et al., *Sequence to Sequence Learning with Neural Networks* (2014)

---

# Day 2 (Tuesday): Attention Mechanism

## Topics
- Why Attention?
- Fixed Context Bottleneck
- Soft Attention
- Alignment Scores
- Context Vector Computation
- Attention Weights
- Interpretability of Attention

## Mathematical Concepts
- Attention score
- Softmax normalization
- Weighted sum of hidden states

## Practical
- Visualize attention weights
- Implement Bahdanau Attention from scratch

## Reading
- Bahdanau et al., *Neural Machine Translation by Jointly Learning to Align and Translate* (2015)

---

# Day 3 (Wednesday): Variants of Attention

## Topics
- Bahdanau (Additive) Attention
- Luong (Multiplicative) Attention
- Global Attention
- Local Attention
- Dot Product Attention
- Scaled Dot Product Attention (Preview)

## Mathematical Concepts
- Dot-product similarity
- Additive attention formulation
- Alignment matrices

## Practical
- Compare Bahdanau and Luong Attention
- Visualize alignment matrices

---

# Day 4 (Thursday): Neural Machine Translation

## Topics
- Machine Translation Pipeline
- Tokenization
- Vocabulary Construction
- Word Embeddings
- Encoder-Decoder Translation
- Beam Search
- Greedy Decoding
- BLEU Score (Introduction)

## Practical
- Train a toy English-to-French translation model
- Evaluate translations using BLEU score

## Reading
- Neural Machine Translation literature overview

---

# Day 5 (Friday): Attention in PyTorch

## Topics
- Implementing Attention Modules
- Attention Layer Design
- Encoder Implementation
- Decoder Implementation
- Teacher Forcing
- Inference Pipeline
- Evaluation Pipeline

## Practical
- Build an Attention-based Seq2Seq model in PyTorch
- Compare results with vanilla Seq2Seq

---

# Day 6 (Saturday): End-to-End Attention-Based NLP System

## Topics
- Complete Seq2Seq Pipeline
- Data Preprocessing
- Vocabulary Generation
- Model Training
- Model Evaluation
- Error Analysis
- Visualization of Attention Maps

## Practical Project

### Option 1: Machine Translation
Dataset:
- Multi30k
- English ↔ German

### Option 2: Text Summarization
Dataset:
- CNN/DailyMail (Subset)

### Pipeline
1. Data Loading
2. Text Preprocessing
3. Vocabulary Building
4. Seq2Seq with Attention
5. Training
6. Evaluation
