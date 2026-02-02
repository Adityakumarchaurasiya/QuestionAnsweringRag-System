# 📚 Question Answering RAG System (PDF-Based)

A **Retrieval-Augmented Generation (RAG)** based Question Answering system that allows users to upload PDF documents and ask questions directly from the content. The system intelligently retrieves relevant information from the document and generates accurate answers using a powerful LLM.

---

## 🚀 Features

- 📄 Upload PDF documents
- ✂️ Automatic text chunking for efficient retrieval
- 🔍 Semantic search using vector embeddings
- 🤖 Context-aware answers powered by LLM
- ⚡ Fast and interactive UI using Streamlit

---

## 🛠️ Tech Stack

- **Frontend**: Streamlit  
- **Backend**: Python  
- **LLM**: Groq – `llama-3.3-70b-versatile`  
- **Framework**: LangChain  
- **Vector Database**: ChromaDB  
- **PDF Loader**: UnstructuredPDFLoader  
- **Text Splitter**: RecursiveCharacterTextSplitter  
- **Embedding & Retrieval**: LangChain Community  
- **QA Chain**: RetrievalQA  

---

## 🧠 How It Works

1. User uploads a PDF file
2. PDF content is extracted using `UnstructuredPDFLoader`
3. Text is split into chunks using `RecursiveCharacterTextSplitter`
4. Chunks are embedded and stored in **ChromaDB**
5. User asks a question
6. Relevant chunks are retrieved
7. Groq LLM generates a precise answer based on retrieved context

---

## 📦 Installation & Setup

```bash
git clone <GITHUB_REPO_LINK>
cd question-answering-rag
pip install -r requirements.txt
streamlit run app.py
