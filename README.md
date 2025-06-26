# 🎓 University RAG Chatbot 
A Production-ready Retrieval-Augmented Generation (RAG) chatbot developed as a capstone project at the University of New Haven. This intelligent assistant leverages semantic search and large language models (LLMs) to answer queries from students and faculty in real time.

> 🚀 Built with FastAPI, Ollama Mistral 7B, ChromaDB, Apache Airflow, and deployed on AWS EC2.

# Chatbot link: http://44.217.147.240:8000 

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
- ✅ Built using Ollama’s Mistral 7B model for fast high quality answers.
- ✅ Vector search with ChromaDB (cosine similarity)
- ✅ Chunked input for semantic search (chunk size = 500, overlap = 100) 
- ✅ Automated scraping + embedding with Airflow DAGs
- ✅ Deployable across institutions with simple config
- ✅ Hosted on GPU-enabled AWS EC2 for optimal performance

# Tech stack

| Component       | Technology            |
| --------------- | --------------------- |
| Embeddings      | all-MiniLM-L6-v2      |
| LLM             | Ollama Mistral 7B     |
| Vector Database | ChromaDB              |
| API Framework   | FastAPI               |
| Scraping        | BeautifulSoup, Scrapy |
| Automation      | Apache Airflow        |
| Cloud Hosting   | AWS EC2 (GPU enabled) |
| Language        | Python                |


# Dataset

📄 Source: University of New Haven website sitemap

📑 Raw: HTML pages with course & faculty info

🔎 Cleaned: 12,000+ chunked text entries (500 tokens each, 100-token overlap)

💾 Stored: In ChromaDB with cosine similarity index


