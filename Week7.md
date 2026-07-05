# Week 7: Transformer Architecture and Pretrained Language Models (BERT & GPT)

## Week Objective

- Understand the limitations of RNNs, LSTMs, and Seq2Seq models
- Learn the Transformer architecture in depth
- Study Self-Attention and Multi-Head Attention
- Understand positional encoding and transformer blocks
- Explore encoder-only and decoder-only language models
- Learn the fundamentals of BERT and GPT
- Build transformer-based NLP models using Hugging Face and PyTorch

---

# Day 1 (Monday): Introduction to Transformers

## Topics
- Limitations of RNNs and LSTMs
- Why Transformers?
- Parallelization in Sequence Modeling
- Overview of the Transformer Architecture
- Encoder-Decoder Transformer
- High-Level Workflow
- Computational Complexity Comparison

## Mathematical Concepts
- Sequence representation
- Matrix multiplication review
- Parallel computation

## Practical
- Visualize the Transformer architecture
- Compare RNN vs LSTM vs Transformer

## Reading
- *Attention Is All You Need* (Sections 1–2)

---

# Day 2 (Tuesday): Self-Attention Mechanism

## Topics
- Query (Q), Key (K), Value (V)
- Self-Attention
- Scaled Dot-Product Attention
- Attention Scores
- Softmax over Attention Scores
- Context Vector
- Multi-Head Attention

## Mathematical Concepts
- Dot Product
- Scaled Dot Product
- Softmax
- Matrix Operations

## Practical
- Implement Self-Attention from scratch using PyTorch
- Visualize attention matrices

## Reading
- *Attention Is All You Need* (Attention Section)

---

# Day 3 (Wednesday): Transformer Encoder and Decoder

## Topics
- Transformer Encoder Block
- Transformer Decoder Block
- Residual Connections
- Layer Normalization
- Feed Forward Networks (FFN)
- Masked Self-Attention
- Cross-Attention
- Encoder-Decoder Interaction

## Mathematical Concepts
- Residual Learning
- Layer Normalization
- Position-wise Feed Forward Networks

## Practical
- Build a Transformer Encoder Block in PyTorch
- Visualize data flow through encoder and decoder

---

# Day 4 (Thursday): Positional Encoding and Language Modeling

## Topics
- Why Positional Encoding?
- Sinusoidal Positional Encoding
- Learned Positional Embeddings
- Causal Language Modeling
- Masked Language Modeling
- Next Token Prediction
- Training Objectives

## Mathematical Concepts
- Sinusoidal encoding equations
- Positional embeddings

## Practical
- Implement positional encoding
- Compare models with and without positional information

## Reading
- Transformer positional encoding section

---

# Day 5 (Friday): Pretrained Language Models — BERT and GPT

## Topics
- What are Foundation Models?
- Transfer Learning in NLP
- Pretraining vs Fine-tuning
- BERT Architecture
- GPT Architecture
- Encoder-only vs Decoder-only Models
- Masked Language Modeling (MLM)
- Causal Language Modeling (CLM)
- Comparison of BERT and GPT
- Applications of Pretrained Language Models

## Practical
- Load pretrained BERT using Hugging Face
- Generate text using GPT
- Perform sentiment analysis using BERT

## Reading
- BERT Paper
- GPT Paper (Overview)

---

# Day 6 (Saturday): Transformers in Practice

## Topics
- Hugging Face Transformers Library
- Tokenizers
- Loading Pretrained Models
- Fine-tuning Workflow
- Inference Pipeline
- Text Classification Pipeline
- Text Generation Pipeline
- Named Entity Recognition Pipeline
- Question Answering Pipeline

## Practical

### Option 1: Text Classification
Dataset:
- IMDB Reviews

### Option 2: Named Entity Recognition
Dataset:
- CoNLL-2003

### Option 3: Question Answering
Dataset:
- SQuAD

### Pipeline
1. Load Dataset
2. Tokenization
3. Load Pretrained Model
4. Fine-tuning
5. Evaluation
6. Inference
