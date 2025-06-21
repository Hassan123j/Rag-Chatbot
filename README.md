# RAG Chatbot

A simple Streamlit app that lets you query PDF documents using Retrieval-Augmented Generation (RAG). Built with LangChain, Groq LLM, HuggingFace embeddings, and ChromaDB.

## Overview

This project enables natural language Q\&A over PDFs. You upload a document, ask questions, and get answers grounded in the content. It uses HuggingFace sentence transformers for embeddings and Groq for fast, low-latency inference.

**Demo:** [LinkedIn Demo](https://shorturl.at/ClGdo)

## Features

* PDF upload and parsing
* Document chunking and vector indexing
* Semantic search with HuggingFace `all-MiniLM-L12-v2`
* Context-aware answering via Groq LLM
* Simple UI built with Streamlit
* .env-based API key configuration

## Stack

* **LLM:** [Groq API](https://console.groq.com)
* **Embeddings:** [HuggingFace Transformers](https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2)
* **Framework:** [LangChain](https://www.langchain.com)
* **Frontend:** [Streamlit](https://streamlit.io)
* **Vector store:** ChromaDB via LangChain

## Setup

Clone the repo:

```bash
git clone https://github.com/Hassan123j/Rag-Chatbot.git
cd Rag-Chatbot
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Set your Groq API key:

```bash
export GROQ_API_KEY=your_api_key_here
```

Or use a `.env` file:

```env
GROQ_API_KEY=your_api_key_here
```

## Run

```bash
streamlit run app.py
```

This will launch the app in your browser. Upload a PDF and start asking questions.

## Project Structure

```
Rag-Chatbot/
├── app.py            # Streamlit frontend
├── requirements.txt  # Dependencies
├── .env              # (optional) API key config
└── README.md         # Project info
```

## Contributing

Feel free to open issues or submit PRs if you have suggestions or improvements.

---

