# Hi, I'm Hamad Alajeel

I'm a Full-stack / Backend Engineer and Machine Learning & Data Science graduate from UC San Diego with a background in Electrical Engineering.

I focus on building AI-driven applications that combine machine learning, backend systems, cloud infrastructure, and MLOps. My work spans computer vision, LLM/RAG pipelines, AI automation, REST APIs, and production-oriented ML deployment.

I am especially interested in AI/ML Engineering, MLOps, Applied Deep Learning, Computer Vision, LLM Applications, and backend systems for AI products.

## Featured Projects

### ApexQ4, End-to-End Investment Analyst Agent









https://github.com/user-attachments/assets/ee877ba3-c5b0-42a4-9733-e01a72eeba5e









ApexQ4 is a production-deployed conversational AI system that answers questions about SEC 10-Q filings for NVIDIA, Microsoft, and Alphabet with page-level inline citations, built to demonstrate the full LLMOps lifecycle from data ingestion and agent design to cloud deployment and observability.

- Designed a two-level LangGraph agent — an orchestrator (`gpt-4o`) that delegates to per-company expert subgraphs (`gpt-4o-mini`) with bounded retrieval loops, keeping persisted session state small while running deep retrieval per query
- Built the ingestion pipeline with Docling's `HybridChunker` and OpenAI `text-embedding-3-small`, preserving page provenance so the agent cites every claim back to the source paragraph
- Persisted per-session chat state in managed Redis Cloud via LangGraph's `RedisSaver` with TTL-based idle expiry
- Built a FastAPI backend and a React + Vite + TypeScript frontend, containerized with a multi-stage Docker image
- Deployed the backend to AWS ECS Fargate behind an ALB with HTTPS termination and application autoscaling; hosted the SPA on S3 + CloudFront with ACM certificates and a Route 53 apex domain
- Codified all AWS infrastructure with Terraform across three independently applied modules (VPC, ECS, IAM, ACM, Route 53, S3, CloudFront)
- Set up CI/CD using GitHub Actions with OIDC (no long-lived AWS keys) for automated tests on `dev`, and separate backend / frontend / vectorstore-rebuild pipelines on `main`
- Wrote 75+ unit and integration tests with pytest, plus a LangSmith LLM-as-judge evaluation pipeline scoring scope adherence and citation grounding

**Tech:** LangGraph, LangChain, OpenAI, Chroma, Docling, Redis, FastAPI, React, TypeScript, Docker, AWS (ECS, ALB, S3, CloudFront, Secrets Manager), Terraform, GitHub Actions, pytest, LangSmith

**Live Demo:** https://apexq4.com

---

### BirdML, End-to-End MLOps Computer Vision System

BirdML is a production-style bird species classification system built to demonstrate the full machine learning lifecycle, from data ingestion and model training to cloud deployment and inference.

- Designed and deployed an end-to-end ML system for a 525-species bird classifier
- Fine-tuned EfficientNet-B3 using AWS SageMaker Processing Steps
- Used Optuna for hyperparameter tuning and MLflow for experiment tracking
- Added a model registry approval step before deployment
- Built a FastAPI inference service and Reflex frontend
- Containerized the application with Docker and deployed it to AWS ECS Fargate behind an Application Load Balancer
- Set up CI/CD using GitHub Actions
- Achieved 99.52% top-1 accuracy and 99.96% top-5 accuracy on the test set

**Tech:** PyTorch, AWS SageMaker, ECS, S3, ECR, FastAPI, Docker, GitHub Actions, MLflow, Optuna, Reflex

**Live Demo:** https://birdml.net

---

### Enhancing Nuclear Safety AI Pipeline, LLM/RAG Document Processing

A research-oriented AI pipeline focused on using LLMs, retrieval-augmented generation, and cache-augmented generation techniques for nuclear safety document workflows.

- Optimized LangChain orchestration logic for a nuclear safety document-lifecycle proof of concept
- Reviewed and improved RAG/CAG pipeline code
- Contributed technical expertise to an AI pipeline for document drafting, verification, and review
- Acknowledged in the resulting research paper for AI pipeline contributions

**Tech:** Python, LangChain, RAG, CAG, ChromaDB, LLMs, Document AI

---

### Academic Projects & SOC Research Contribution

My academic projects include applied machine learning, deep learning, simulation, optimization, and systems-oriented work from my Electrical Engineering and Machine Learning background.

One of my pinned contributions is to the UCSD SOC research group repository, where I contributed Julia implementations of mixed traffic simulations based on SOC research papers. The work focuses on Connected Autonomous Vehicle control in mixed traffic flow, formulating traffic control as a convex optimization problem.

- Implemented mixed traffic simulation experiments in Julia
- Worked with convex optimization tools and conic solvers
- Used packages such as Convex.jl, MosekTools.jl, PyPlot, CSV, DataFrames, and LinearAlgebra
- Connected research papers on autonomous vehicle formation control with executable simulation notebooks
- Also maintain related academic project work in my Academic-Projects repository

**Tech:** Julia, Convex Optimization, MosekTools, Jupyter, Traffic Simulation, Autonomous Vehicles

## Experience

### Settlyfe Inc., Full-stack / Backend Engineer

I build and maintain backend services for production application features using Java Spring Boot, MySQL, and RESTful APIs. My work includes roommate matching, swipe interactions, top-match selection logic, database schema improvements, and Git-based team development.

### Revscale Technologies Inc., AI Automation Intern

I built AI automation workflows using tools such as n8n, Zapier, APIs, vector databases, and LLM pipelines. My work included RAG data pipelines, AI voice agent scheduling improvements, campaign reporting automation, and centralized error monitoring.

## Technical Skills

**Machine Learning & AI:** Deep Learning, Computer Vision, NLP, Generative AI, LLMs, RAG, Agentic AI, AI Automation, Vector Databases  
**Programming:** Python, Java, SQL, C, C++, MATLAB, Verilog, SystemVerilog, Julia  
**ML Frameworks:** PyTorch, TensorFlow, Scikit-learn, Optuna, LangChain  
**MLOps & Cloud:** AWS SageMaker, ECS, S3, ECR, Docker, GitHub Actions, CI/CD, MLflow, Azure ML  
**Backend:** FastAPI, Spring Boot, REST APIs, MySQL, Redis, MyBatis  
**Automation & AI Tools:** Pinecone, ChromaDB, n8n, Zapier, VAPI, Microsoft Copilot  
**Other:** Git, Data Engineering, ETL, Data Preprocessing, Data Visualization

## Education

**University of California San Diego**  
M.S. in Machine Learning and Data Science

**University of California San Diego**  
B.S. in Electrical Engineering

## Contact

- GitHub: https://github.com/Hamad-Alajeel
- LinkedIn: [https://linkedin.com/in/hamad-alajeel](https://www.linkedin.com/in/hamad-alajeel-a6bb41210/)
- Email: hamad.alajeel2019@gmail.com
