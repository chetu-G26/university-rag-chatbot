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

🔍 Smart Web Scraper

Automatically scrapes university content using sitemap-based filtering, ensuring relevant and structured data extraction.

🧠 Efficient Embedding with ChromaDB

Uses all-MiniLM-L6-v2 for document embeddings.

Enables powerful semantic understanding of content.

💬 Interactive Chat Interface

A simple and intuitive web-based chatbot for querying embedded documents.

Fast, responsive, and ideal for real-time Q&A.

🔍 Vector Search with ChromaDB

Implements high-speed vector search for accurate information retrieval.

Optimized for semantic relevance and low-latency response.

💬 LLM-Powered Chat

Integrated with Ollama’s Mistral 7B, delivering fast and high-quality answers with natural language understanding.

🧩 Smart Chunking Strategy

Inputs are split into chunks of 500 tokens with 100-token overlap for precise context-aware search results.

⚙️ Automated Monthly Refresh with Airflow

Airflow DAG automates monthly data refresh to keep the knowledge base up to date with new content.

🎛️ Zero-Code Configuration

Fully customizable through config.yaml.

No code modifications needed to update URLs, chunk size, embedding model, etc.

🔴 Real-time Learning

Continuously updates vector store with newly extracted documents, adapting to fresh content automatically.

☁️ Cloud Deployment Ready

Easily deployable on cloud platforms like AWS, GCP, Azure, or Render.
