# LennyHub RAG Explorer

## Overview
A Streamlit-based web application for querying and exploring podcast transcripts using a RAG (Retrieval-Augmented Generation) system with Qdrant vector database.

## Project Structure
- `streamlit_app.py` - Main Streamlit web application
- `query_rag.py` - RAG query functionality
- `build_transcript_rag.py` - Build RAG index from transcripts
- `qdrant_config.py` - Qdrant vector database configuration
- `data/` - Transcript data directory
- `rag_storage/` - RAG storage directory
- `.streamlit/config.toml` - Streamlit configuration

## Running the App
The app runs via Streamlit on port 5000:
```bash
streamlit run streamlit_app.py
```

## Requirements
- Python 3.11
- OpenAI API key (for embeddings and LLM)
- Qdrant vector database (optional, app works without it)

## Environment Variables
- `OPENAI_API_KEY` - Required for RAG queries
- `QDRANT_URL` - URL for Qdrant server (default: http://localhost:6333)
- `QDRANT_COLLECTION_NAME` - Qdrant collection name (default: lennyhub)
- `USE_QDRANT` - Set to 'true' to use Qdrant

## Recent Changes
- January 20, 2026: Configured for Replit environment with Streamlit on port 5000
