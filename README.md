# Semantic Search and ReRank with Transformers

This project provides a simple implementation of semantic search and reranking using transformers, specifically bi-encoders and cross-encoders. The main goal is to provide more accurate and relevant search results for a given query. It is based on Hugging Face's transformers library and Sentence Transformers library, and leverages the Simple Wikipedia dataset for search.

## Installation

To install the required dependencies, run:

```bash
pip install huggingface-hub
pip install datasets
pip install transformers
pip install sentence-transformers
pip install faiss-gpu
pip install faiss-cpu
pip install gradio
```

## Usage

To use the provided code, simply run the entire script. It will start by installing the required packages, followed by importing the necessary modules, and finally launching a Gradio interface. In this interface, you can enter a query and see the reranked search results.

## Implementation

The implementation consists of the following steps:

1. Import required packages and modules.
2. Load bi-encoder and tokenizer.
3. Load cross-encoder and tokenizer.
4. Load the Simple Wikipedia dataset and convert it into a Hugging Face dataset.
5. Create embeddings for the dataset using the bi-encoder.
6. Push the dataset with embeddings to Hugging Face Hub.
7. Load the dataset from Hugging Face Hub.
8. Add a FAISS index for efficient search.
9. Define a function to rerank search results using cross-encoder.
10. Create a Gradio interface for user input and display of search results.

## Acknowledgements

This project uses the following resources:

- [Hugging Face transformers library](https://github.com/huggingface/transformers)
- [Sentence Transformers library](https://github.com/UKPLab/sentence-transformers)
- [Simple Wikipedia dataset](https://simple.wikipedia.org/wiki/Simple_English_Wikipedia)
- [Gradio](https://www.gradio.app/)
