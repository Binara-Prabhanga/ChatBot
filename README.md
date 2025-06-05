# 📄 Conversational Document-Aware Chatbot

This project is a context-aware chatbot built using **Retrieval-Augmented Generation (RAG)** architecture. It allows users to upload documents (PDF, DOCX, TXT) and ask questions related to their content. The system retrieves relevant parts of the document and uses a **Large Language Model (LLM)** to generate accurate and contextual answers.

## 🚀 Features

- Upload and process `.txt` documents
- Ask natural language questions about the uploaded document
- Relevant context is retrieved automatically
- Uses **Google Gemini Pro** for generation
- Uses **Vertex AI Embeddings** for semantic search
- Based on **LangChain** and **RAG architecture**
- Designed to be scalable and cloud-integrated

## 🧠 LLM Strategy

- **Initial model:** OpenAI GPT (faced token and quota limitations)
- **Final model:** Google Gemini Pro (better context window, free-tier access, better GCP integration)

## 🔧 Tech Stack

- **Language Model:** Google Gemini Pro via AI Studio
- **Embeddings:** Vertex AI (Google Cloud)
- **Frameworks:** LangChain, Python
- **Deployment:** Google Cloud Platform (GCP)
- **Document Processing:** LangChain Document Loaders
- **Frontend (optional):** Streamlit / Flask (optional)

## 📌 How It Works

1. Upload a document (currently supports `.txt`)
2. The text is embedded and indexed using vector search
3. User submits a question
4. Top-k relevant text chunks are retrieved
5. Prompt is constructed with retrieved context + question
6. Gemini generates an answer using RAG pipeline

## ⚠️ Limitations

- Currently supports `.txt` files only (can be extended)
- No chat history / multi-user support (planned for future)
- API limits may still apply on free tier

## 📚 Use Cases

- Document Q&A assistants
- Educational LMS bots
- Legal/HR document support
- Research assistants

## 📄 Author

**IT21211096 - Prabhanga K.G.B**  
Sri Lanka Institute of Information Technology (SLIIT)  
Module: SE4010 - Current Trends in Software Engineering

