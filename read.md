AgenticDocAI – RAG-Based Document Intelligence Platform | Python, LangChain, Streamlit, FAISS, OpenAI, Groq (Llama 3.1), LangSmith

Built a retrieval-augmented generation (RAG) app that lets users upload PDF, DOCX and TXT files and ask questions about them in plain English. Answers are grounded in the most relevant passages from those documents.
Built the ingestion pipeline with LangChain document loaders and recursive character chunking (1,000-character chunks, 200 overlap). Text is embedded with OpenAI embeddings into a FAISS vector index.
Embedded documents in batches and merged them into one index to stay under API rate limits, with automatic retries, live progress tracking and the ability to save and reload the index.
Built the answer pipeline with LangChain retrieval and “stuff documents” chains on Groq-hosted Llama 3.1. Users can switch models and adjust temperature, max tokens and top-k.
Added three ways to search (similarity, MMR, score-threshold) so users can trade answer precision against variety in the retrieved context.
Split the code into modules for document processing, the vector store, chat, validation and config. Added checks on API keys, file size and type, user input and model/retrieval settings.
Built a Streamlit interface with chat history, response-time analytics, chat export and a settings panel.
Added a second, general-purpose chatbot built with LangChain prompt chains (prompt → model → output parser) on OpenAI, with LangSmith tracing to monitor and debug what the model is doing.
