# 🔍 Agentic RAG with LangGraph + FAISS + Cohere + OpenAI

This project demonstrates a simple **3-agent Retrieval-Augmented Generation (RAG)** system using:

- 🧠 **LangGraph** for agent workflow orchestration
- 📚 **FAISS** for vector similarity search
- 🎯 **Cohere Rerank** for contextual reranking
- 💬 **OpenAI GPT-3.5** for final answer generation

---

## 📌 How It Works

The pipeline follows this flow:

1. **Retriever Agent**
   - Uses `FAISS` to retrieve top 10 similar chunks based on user query.
   
2. **Reranker Agent**
   - Uses `Cohere Rerank API` to refine and reorder the chunks for better relevance.

3. **Answer Agent**
   - Uses `OpenAI ChatGPT` to generate a final answer using the top reranked documents.

*** Technologies Used
LangGraph

LangChain

FAISS

Cohere Rerank

OpenAI GPT-3.5


```mermaid
graph TD
retriever_agent --> reranker_agent --> answer_agent --> END



