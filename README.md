# RAG Chatbot API with FastAPI

## Overview

A production-ready Retrieval-Augmented Generation (RAG) chatbot API built with FastAPI.

### Key Features
- Chat endpoint with RAG-enhanced responses  
- Document upload and indexing  
- Document management  
- High-performance API  
- Robust error handling  

## Getting Started

### Prerequisites
- Python 3.8+  
- Understanding of:  
  - Python and async programming  
  - RESTful APIs  
  - RAG systems and LangChain  
  - FastAPI  

### Project Structure
rag-fastapi-project/
│
├── main.py                 # FastAPI application entry point
├── chroma_utils.py         # Chroma vector store utilities
├── db_utils.py             # Database operations
├── langchain_utils.py      # LangChain configuration
├── pydantic_models.py      # Data models
├── requirements.txt        # Project dependencies
└── chroma_db/              # Chroma persistence directory

### Installation

1. Create and activate virtual environment:
python -m venv .venv
.\.venv\Scripts\activate  # Windows

2. Install dependencies:
pip install -r requirements.txt

### Configuration
1. Create a .env file  
2. Add required API keys and settings  

### Launch
uvicorn main:app --reload

## API Endpoints

- POST /chat: Process queries using RAG system  
- POST /documents: Upload and index documents  
- GET /documents: List indexed documents  
- DELETE /documents/{doc_id}: Remove documents  

## Components

- Vector Store: Chroma for similarity search  
- LangChain Integration: RAG chain setup  
- Document Processing: Multi-format support  
- Data Validation: Pydantic models  

## Development

### Core Modules
- main.py: API routes  
- chroma_utils.py: Vector operations  
- db_utils.py: Database layer  
- langchain_utils.py: LangChain setup  
- pydantic_models.py: Data models  

### Dependencies
- langchain  
- langchain-openai  
- fastapi  
- uvicorn  
- View full list in requirements.txt  



Visit /docs or /redoc after starting the server.
