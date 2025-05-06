# Rag-Chatbot
 A Streamlit-based AI chatbot that reads PDFs and answers user questions using LangChain, HuggingFace embeddings, Groq LLM, and Retrieval-Augmented Generation (RAG).

 # PDF Chatbot using LangChain, HuggingFace & Groq

This project is an AI-powered chatbot built with **LangChain**, **Groq LLM**, and **Streamlit**, designed to intelligently read a PDF document and answer user queries using the content of that document.

##  Features

-  Upload and read PDF documents
-  Chunk the document into searchable vectors
-  Retrieve accurate answers using Groq's LLM
-  Uses HuggingFace Embeddings (`all-MiniLM-L12-v2`)
-  Clean and interactive chat UI with Streamlit
-  Environment variable-based API key handling

---

## 🛠 Tech Stack

| Component       | Library/API               |
|----------------|---------------------------|
| LLM             | Groq API https://console.groq.com            |
| Embeddings      | HuggingFace Transformers https://huggingface.co/sentence-transformers/all-MiniLM-L12-v2 |
| Framework       | LangChain https://www.langchain.com/           |
| Frontend        | Streamlit https://streamlit.io/                |
| PDF Parsing     | `PyPDFLoader` from LangChain                      |
| Vector DB       | `VectorstoreIndexCreator` ChromaDB backend      |

---

## Installation

git clone https://github.com/Hassan123j/Rag-Chatbot.git
cd Rag-Chatbot
pip install -r requirements.txt

Set your environment variable for Groq API:

export GROQ_API_KEY=your_groq_api_key

 Run the App

streamlit run app.py

Project Structure
.

├── app.py               # Main Streamlit application
├── requirements.txt     # Python dependencies
└── README.md            # You're here!


