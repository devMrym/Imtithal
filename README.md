# Imtithal – Smart Dynamic Arabic Compliance Chatbot

A **Retrieval-Augmented Generation (RAG)** system designed to analyze Saudi regulatory documents (SDAIA & NCA) and answer user queries in Arabic. The assistant combines **semantic search, keyword search, query rewriting, and LLM reasoning** to provide accurate and context-aware responses.  

---

## 📝 Project Overview

This project allows users to:

- Ask questions in Arabic related to Saudi regulatory frameworks.
- Handle **follow-up questions** intelligently using query classification and rewriting.
- Retrieve relevant sections from a **ChromaDB vector database** using a **hybrid semantic + keyword search**.
- Rerank documents for precise responses.
- Display sources alongside answers for transparency.

The system supports **interactive chat sessions** via a Django web interface, allowing users to upload and query regulatory PDFs.

---

## ⚙️ Features

- **Arabic Text Cleaning** – Normalizes Arabic text (removes diacritics, elongations, and extra whitespace).  
- **Query Classification** – Detects if a question is new or a follow-up.  
- **Query Rewriting** – Converts follow-ups into standalone queries for better retrieval.  
- **Hybrid Retriever** – Combines semantic embeddings and BM25 keyword search.  
- **Reranker** – Ranks retrieved documents by similarity to the query.  
- **Dynamic Prompting** – LLM prompts adapt based on whether a query is a follow-up.  
- **Interactive Chat** – Users can ask questions through a web interface and see sources.  
