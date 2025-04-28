# Sorting Transformer

A simple transformer-based neural network model that learns to sort sequences of integers.

## Overview

This code is a minimal implementation that shows how a Transformer architecture can learn to sort integer sequences using attention mechanisms to understand the relationships between elements in a sequence.

## Features

* Generates random integer sequences and their sorted counterparts
* Implements a basic transformer with:
   * Custom embedding layer combining token and positional embeddings
   * Self-attention mechanism
   * Transformer encoder layers with residual connections
   * Classification head for prediction

## Requirements

* PyTorch
* Matplotlib
* Numpy

## Model Architecture

The model consists of:
* `IntegerSequenceEmbedding`: Combines token and positional embeddings
* `SingleHeadAttention`: Implements the self-attention mechanism
* `TransformerEncoderLayer`: A single transformer encoder layer with attention and feed-forward network
* `Transformer`: The complete model with embedding, encoder layers, and output layer

## Usage

Run the main script to train and evaluate the model:

```python
python sorting_transformer.py
```
## Configuration
You can adjust the following parameters in the main() function:

* vocab_size: Maximum value of integers in the sequence (default: 20)
* embed_dim: Embedding dimension (default: 64)
* seq_length: Length of the sequences to sort (default: 10)
* num_layers: Number of transformer encoder layers (default: 3)
* batch_size: Training batch size (default: 64)
* num_epochs: Number of training epochs (default: 300)
