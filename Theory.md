AI-Powered Legal Compliance Assistant
Overview

The AI-Powered Legal Compliance Assistant is a Legal Tech solution developed as part of my Master's thesis at the University of Bonn. The project applies Retrieval-Augmented Generation (RAG) and Large Language Models (LLMs) to assist organizations in answering regulatory and compliance-related questions directly from legal documents.

Instead of manually searching through lengthy regulations, contracts, or policy documents, users can ask questions in natural language and receive evidence-grounded responses generated from the most relevant legal sources.

Business Problem

Legal and compliance teams spend significant time searching through regulations and legal documents to answer compliance-related questions. Traditional keyword-based search often requires manual interpretation, making the process slow, inconsistent, and resource-intensive.

Organizations need a solution that enables employees to quickly access reliable regulatory information while ensuring responses remain grounded in authoritative legal documents.

Solution

This project implements a Retrieval-Augmented Generation (RAG) pipeline that combines semantic document retrieval with Large Language Models to generate accurate, context-aware responses.

The system:

Retrieves the most relevant legal passages
Generates evidence-based answers
Reduces manual legal research
Supports compliance decision-making
Improves access to regulatory knowledge
Key Features
AI-powered regulatory question answering
Semantic legal document retrieval
Evidence-grounded response generation
Multiple prompting strategies
Retrieval model benchmarking
Compact LLM evaluation
Automated performance evaluation using legal QA metrics
Technical Architecture
User Question
       │
       ▼
Embedding Model
       │
       ▼
Vector Database
       │
Retrieve Relevant Legal Documents
       │
       ▼
Prompt Construction
       │
       ▼
Large Language Model
       │
       ▼
Evidence-Based Compliance Answer
Technologies
Retrieval
BM25
BGE
ColBERT
NV-Embed
SPLADE
Large Language Models
Qwen 2.5
Gemma 2
DeepSeek R1 Distill
Mistral
AI Techniques
Retrieval-Augmented Generation (RAG)
RAFT (Retrieval-Augmented Fine-Tuning)
LoRA Fine-Tuning
Few-shot Prompting
Chain-of-Thought Prompting
Development
Python
PyTorch
Hugging Face Transformers
Sentence Transformers
FAISS
Google Colab
Evaluation

The system was evaluated on public legal question answering datasets including:

ObliQA
Open Australian LegalQA
CUAD

Performance was assessed using legal-domain evaluation metrics such as:

Obligation Coverage
Entailment Score
Contradiction Score
RePASs
Business Impact

This project demonstrates how AI can support Legal Tech by:

Reducing manual legal research
Improving access to regulatory information
Supporting compliance workflows
Providing evidence-grounded legal responses
Enabling faster compliance decision-making

Note: The system is designed to assist legal professionals, not replace legal expertise. Final legal decisions should always be reviewed by qualified professionals.

Future Improvements
Contract analysis
Clause extraction
Risk identification
Multi-document reasoning
Integration with enterprise document management systems
Microsoft Copilot integration
Legal chatbot interface
