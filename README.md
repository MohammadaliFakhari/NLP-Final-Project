# Textbook Q&A with RAG

A Retrieval-Augmented Generation (RAG) system designed to answer questions from a human nutrition textbook. This project demonstrates the implementation of RAG from scratch, including document retrieval and response generation using advanced language models.

## Features

- **Corpus Processing**: Extracts and chunks text from a PDF textbook for efficient retrieval.
- **Query Handling**: Supports 20 nutrition-related queries with context-aware responses.
- **Multi-Model Comparison**: Evaluates three state-of-the-art LLMs (Llama-3, StableBeluga, Gemma) for response quality.
- **Evaluation Framework**: Uses a judge model to rank responses and determine the best-performing model.

## Models Used

1. **NousResearch/Meta-Llama-3-8B-Instruct**
2. **stabilityai/StableBeluga-7B**
3. **google/gemma-7b-it**

## Results

The system retrieves relevant document chunks and generates answers, with evaluation metrics comparing the performance of each model. Results are stored and analyzed to determine the most effective generator for the task.

## Setup

```bash
pip install PyMuPDF sentence-transformers accelerate bitsandbytes transformers datasets huggingface_hub
