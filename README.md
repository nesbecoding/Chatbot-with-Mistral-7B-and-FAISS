# RAG Chatbot with Mistral-7B and FAISS

## Description

A question-answering chatbot built on a RAG pipeline. The system encodes a knowledge base of Amazon Q&A pairs into vector embeddings, retrieves context using **FAISS**, and generates grounded answers using **Mistral-7B-Instruct**.

This project compares two variants:
- **Stateless:** Answers queries based only on the current prompt.
- **Memory-Augmented:** Uses conversation history to resolve follow-up questions and maintain consistency.

All models are free and open-source.

## Objective

- Build a functional RAG pipeline using open-source tools
- Compare stateless vs. memory-augmented answer generation
- Show how including conversation history helps the model resolve follow-up questions correctly

## Requirements

```bash
python -m pip install numpy transformers datasets sentence-transformers faiss-cpu torch
```

A GPU is required to load Mistral-7B in float16
