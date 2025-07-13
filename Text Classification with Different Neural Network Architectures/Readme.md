# Project README

## Datasets
This project works with three different datasets for text classification and sentiment analysis:

- **IMDB Movie Reviews:** Binary sentiment classification (positive/negative)
- **Persian Text Sentiment:** Sentiment analysis for Persian texts
- **Persian News Dataset:** Categorization of Persian news articles

---

## Architectures
The project implements several neural network architectures divided into four main parts:

### Part 1: Basic Embedding
- Uses a simple embedding layer followed by dense layers
- Tested with various embedding dimensions: 10, 32, 64, 100

### Part 2: Pre-trained Embeddings
- Employs GloVe (Global Vectors for Word Representation) embeddings
- Embedding layer initialized with pre-trained weights for better representation

### Part 3: SimpleRNN
- Implements Recurrent Neural Networks using SimpleRNN layers
- Supports stacked RNN layers to build deeper architectures

### Part 4: LSTM
- Uses Long Short-Term Memory (LSTM) networks for sequence modeling
- Includes bidirectional LSTM implementations to capture context from both directions

---

## Installation
To run the code, ensure you have the following packages installed:

```bash
pip install tensorflow datasets gensim scikit-learn numpy
