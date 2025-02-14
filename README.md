# nn-text-gen

This repository contains PyTorch implementations of neural networks for text generation. Specifically, it includes an RNN-based character-level model and a Transformer-based model trained on classic literary texts from Project Gutenberg.

## Models Implemented

### 1. Transformer Model
A Transformer-based text generator leveraging self-attention mechanisms and positional encodings.
- **Architecture**:
  - Token embedding layer
  - Positional encoding
  - Transformer encoder with multiple layers
  - Fully connected output layer
- **Key Parameters**:
  - `ntoken`: Vocabulary size
  - `ninp`: Embedding dimension
  - `nhead`: Number of attention heads
  - `nhid`: Hidden layer size
  - `nlayers`: Number of transformer layers
  - `dropout`: Dropout rate

### 2. Character-Level RNN
A simple recurrent neural network for character-level text generation.
- **Architecture**:
  - RNN layer (vanilla RNN)
  - Fully connected output layer
- **Key Parameters**:
  - `input_size`: Vocabulary size
  - `hidden_size`: Number of hidden units
  - `output_size`: Vocabulary size
 
### Model Architecture Derived From: 
- https://github.com/pytorch/examples/blob/main/word_language_model/model.py

## Training Data
The models are trained on the following classic texts from Project Gutenberg:
- *Shakespeare's Complete Works* ([Link](https://www.gutenberg.org/files/100/100-0.txt))
- *War and Peace* by Leo Tolstoy ([Link](https://www.gutenberg.org/files/2600/2600-0.txt))
- *Moby-Dick* by Herman Melville ([Link](https://www.gutenberg.org/ebooks/2701.txt.utf-8))

## Future Improvements
- Implement word-level tokenization for improved text generation.
- Add pre-trained embeddings (e.g., GloVe, Word2Vec) to enhance input representations.
- Fine-tune hyperparameters for better performance.

## Acknowledgments
This project utilizes open-source datasets from Project Gutenberg and PyTorch for model implementation.
