# PDF RAG/SAG/CAG Demo

This project demonstrates **Retrieval-Augmented Generation (RAG)**, **Self-Augmented Generation (SAG)**, and **Context-Augmented Generation (CAG)** on a library of PDFs using **ChromaDB**, **SentenceTransformers embeddings**, and **Gemini / LLM** for generation.

---

## **Overview**

The system allows you to:

1. Upload PDFs or point to local PDF files.
2. Extract text and chunk it intelligently using sentence-based token splitting.
3. Embed chunks and store them persistently in **ChromaDB**.
4. Perform semantic search using vector similarity.
5. Generate answers using:
   - **RAG**: Direct retrieval + generation
   - **SAG**: Decompose question → retrieve → sub-answer → aggregate
   - **CAG**: Summarize each chunk → generate final answer

---

## **Setup & Installation**

```bash
pip install PyPDF2
pip install sentence-transformers
pip install chromadb
pip install langchain-community
pip install google-generativeai   # Gemini LLM
pip install python-dotenv         # Optional for API keys
