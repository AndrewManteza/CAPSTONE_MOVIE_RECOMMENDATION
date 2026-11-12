# RAG Chatbot Projects

Retrieval-augmented generation (RAG) chatbot built on Databricks with Unity Catalog Vector Search, LangChain, and Databricks-hosted LLMs.

## Movie Recommendation RAG (Capstone)

- Ingests movie CSVs, chunks text, and indexes it with Databricks Vector Search
- LangGraph pipeline: retrieve, generate, grade answer, with a DuckDuckGo web fallback when the answer is unhelpful
- Randomized recommendations: retrieves a wide pool, samples a varied set per call
- LangGraph MemorySaver for conversation memory, with optional Delta table analytics logging
- Deployed as an MLflow model behind a Databricks serving endpoint, with a Next.js/Vercel chat frontend
- Keep-alive job pings and warms the endpoints every 5 days

