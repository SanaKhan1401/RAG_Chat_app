# RAG_Chat_app
# Streamlit RAG App

A Streamlit application demonstrating a Multi-Document Retrieval-Augmented Generation (RAG) pipeline. Upload files (CSV, XLSX, JSON, PDF, DOCX, PPTX, TXT), the app will ingest them, chunk text, build embeddings using sentence-transformers, store in FAISS, and answer questions via a retrieval+LLM chain.
## Features
- Upload multiple files (structured and unstructured)
- Document ingestion and preprocessing
- Chunking with overlaps
- Embeddings using `sentence-transformers/all-MiniLM-L6-v2`
- Vector store using FAISS (in-memory)
- Simple Streamlit chat interface
- Shows top retrieved context chunks for transparency
## Requirements
- Python 3.10+
## Setup
1. Create virtualenv and activate
```bash
python -m venv .venv
source .venv/bin/activate # macOS / Linux
.venv\Scripts\activate # Windows
