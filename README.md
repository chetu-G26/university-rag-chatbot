# 🎓 University RAG Chatbot 
A Production-ready Retrieval-Augmented Generation (RAG) chatbot developed as a capstone project at the University of New Haven. This intelligent assistant leverages semantic search and large language models (LLMs) to answer queries from students and faculty in real time.

> 🚀 Built with FastAPI, Ollama Mistral 7B, ChromaDB, Apache Airflow, and deployed on AWS EC2.

Chatbot link: http://44.217.147.240:8000 

## 📌 Project Overview

This chatbot system automates student/faculty Q&A using a modern NLP pipeline:
- Scrapes university website data
- Cleans and chunks text
- Embeds chunks with MiniLM
- Stores vectors in ChromaDB
- Uses LLM (Mistral 7B) to generate responses
- Updates monthly with Apache Airflow


## 🧠 Key Features

- ✅ Real-time answers with semantic understanding
- ✅ Built using Ollama’s Mistral 7B model
- ✅ Vector search with ChromaDB (cosine similarity)
- ✅ Automated scraping + embedding with Airflow DAGs
- ✅ Deployable across institutions with simple config
- ✅ Hosted on GPU-enabled AWS EC2 for optimal performance

---

## 🧱 Architecture

```plaintext
         +-------------+ 
         |   User      |
         +------+------+
                |
          [FastAPI App]
                |
    +-----------v-----------+
    |  Retrieve top chunks  |
    |   from ChromaDB DB    |
    +-----------+-----------+
                |
          [Ollama LLM API]
                |
         +------v------+
         |  Final Answer |
         +-------------+
