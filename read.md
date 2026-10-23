AgenticDocAI – RAG-Based Document Intelligence Platform | Python, LangChain, Streamlit, FAISS, OpenAI, Groq (Llama 3.1), LangSmith

Built a retrieval-augmented generation (RAG) app that lets users upload PDF, DOCX and TXT files and ask questions about them in plain English. Answers are grounded in the most relevant passages from those documents.
Built the ingestion pipeline with LangChain document loaders and recursive character chunking (1,000-character chunks, 200 overlap). Text is embedded with OpenAI embeddings into a FAISS vector index.
Embedded documents in batches and merged them into one index to stay under API rate limits, with automatic retries, live progress tracking and the ability to save and reload the index.
Built the answer pipeline with LangChain retrieval and “stuff documents” chains on Groq-hosted Llama 3.1. Users can switch models and adjust temperature, max tokens and top-k.
Added three ways to search (similarity, MMR, score-threshold) so users can trade answer precision against variety in the retrieved context.
Split the code into modules for document processing, the vector store, chat, validation and config. Added checks on API keys, file size and type, user input and model/retrieval settings.
Built a Streamlit interface with chat history, response-time analytics, chat export and a settings panel.
Added a second, general-purpose chatbot built with LangChain prompt chains (prompt → model → output parser) on OpenAI, with LangSmith tracing to monitor and debug what the model is doing.


----------------------
# PROFESSIONAL SUMMARY

AI-focused software engineer and PhD student in Computer Science with experience in full-stack development, AI/ML engineering, retrieval-augmented generation (RAG), document intelligence, and model inference optimization. Hands-on experience with Python, PyTorch, GPU computing, LLM inference, quantization, latency benchmarking, LangChain, and LangGraph. Experienced in developing backend APIs, cloud-based services, database-driven applications, and production monitoring workflows. Interested in building scalable agentic AI systems, efficient model-serving infrastructure, and reliable AI-powered applications.

# TECHNICAL SKILLS

**Programming Languages:** Python, SQL, JavaScript/TypeScript

**AI/ML:** PyTorch, Natural Language Processing (NLP), Embeddings, Semantic Search, Retrieval-Augmented Generation (RAG), Document Intelligence, Model Inference, Quantization, Latency Benchmarking

**LLM and Agentic Frameworks:** LangChain, LangGraph, vLLM, LLM Integration, Tool/API Orchestration, Multi-Step AI Workflows

**GPU and Performance Engineering:** GPU Computing, Inference Optimization, P95/P99 Latency Analysis, Model Performance Evaluation

**Backend and Cloud:** FastAPI, REST APIs, AWS Lambda, Amazon Kinesis, Amazon S3, Docker, Kubernetes, Amazon EKS, AWS IAM

**Data and Retrieval:** PostgreSQL, FAISS, Vector Search, Snowflake, Document Processing, Metadata Filtering

**Monitoring and Observability:** New Relic, Splunk, Observe, Amazon CloudWatch, Application Performance Monitoring, Production Troubleshooting

**Development Practices:** Unit Testing, Integration Testing, API Validation, Agile Development, CI/CD

# PROFESSIONAL EXPERIENCE

## Capital One
**Full Stack Developer — Contractor** | [Start Date] – Present

- Develop and maintain full-stack application functionality, integrating frontend components with backend APIs and database-driven services.
- Build and support backend API integrations to enable reliable communication between application components and data services.
- Monitor application health and investigate production issues using New Relic, Splunk, Observe, and Snowflake.
- Analyze P95 and P99 latency metrics to identify performance bottlenecks and investigate application response-time issues.
- Troubleshoot issues across frontend, backend, and database layers to support application reliability and performance.
- Collaborate with team members to diagnose defects, validate changes, and maintain application quality.

## ADP
**AI/ML Engineer** | June 2021 – August 2022

- Developed Python and FastAPI microservices to support internal knowledge retrieval through REST APIs.
- Built AWS-based data ingestion workflows using Lambda, Kinesis, and S3 to process and prepare documents for downstream retrieval.
- Implemented document chunking, embedding generation, and metadata processing to support semantic search and information retrieval.
- Developed retrieval and ranking workflows to identify relevant document passages and associate results with their source content.
- Applied metadata-based access filtering and input validation to support controlled and reliable retrieval.
- Containerized services using Docker and supported deployment and operations in Kubernetes/EKS environments.
- Used CloudWatch monitoring and AWS IAM controls to support operational visibility and access management.
- Collaborated with stakeholders to review retrieval relevance, test service behavior, and support iterative releases.
- Wrote and maintained unit and integration tests to validate API behavior and retrieval functionality.

# AI PROJECTS

## AgenticDocAI — RAG-Based Document Intelligence Platform
**Technologies:** Python, LangChain, Streamlit, FAISS, OpenAI, Groq, Llama 3.1

- Built a document-question-answering application that accepts PDF, DOCX, and TXT files and generates answers grounded in retrieved document content.
- Implemented document loading, recursive text chunking, embedding generation, and FAISS-based vector indexing for semantic retrieval.
- Integrated an LLM-based response-generation pipeline using LangChain and Groq-hosted Llama models.
- Implemented configurable retrieval strategies, including similarity search, maximal marginal relevance (MMR), and score-threshold retrieval.
- Added batched embedding processing, retry handling, progress feedback, and vector-index persistence to support document ingestion workflows.
- Developed an interactive Streamlit interface with conversational history, model settings, retrieval configuration, response analytics, and export functionality.
- Organized application components into reusable modules and implemented validation for user inputs, uploaded files, and API interactions.

## LLM Inference and Performance Optimization
**Technologies:** PyTorch, GPU, vLLM

- Evaluated LLM inference performance across tested configurations and analyzed response latency.
- Used P95 and P99 latency measurements to assess inference performance and identify opportunities for optimization.
- Explored model quantization and inference optimization techniques to evaluate their impact on latency and resource usage.
- Compared model-serving configurations using consistent workloads and documented performance trade-offs.

## Agentic AI Workflow Engineering
**Technologies:** Python, LangGraph, LangChain

- Developed multi-step AI workflows that use tool or API calls to perform tasks across multiple stages.
- Implemented workflow routing and state management to coordinate task execution.
- Incorporated error handling and workflow validation to improve execution reliability.
- Evaluated workflow behavior using representative tasks and reviewed results to identify opportunities for improvement.

# EDUCATION

## University of Missouri–Kansas City (UMKC)
**Ph.D. in Computer Science — Artificial Intelligence** | August 2026 – Present

**Master of Science in Computer Science — AI Focus** | [Graduation Date]
