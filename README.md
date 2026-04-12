# Regulatory Question Answering using RAG and LLMs

## Overview
This repository contains my Master's thesis project on **Retrieval-Augmented Generation (RAG)** for **regulatory and legal question answering**.

The system is designed to retrieve relevant regulatory passages and generate **factually grounded, context-aware answers** using Large Language Models (LLMs).

---

## Objectives
- Build an end-to-end **RAG pipeline** for regulatory QA
- Improve retrieval using **domain-specific models (LegalBERT, E5, BGE)**
- Develop **robust answer generation** using LLMs
- Evaluate answer quality using advanced metrics like **RePAS**

---

## System Architecture

The pipeline consists of two main components:

1. **Passage Retrieval**
   - Dense retrieval (LegalBERT, SentenceTransformers)
   - BM25 lexical retrieval
   - Hybrid retrieval (Dense + BM25)

2. **Answer Generation**
   - LLM-based generation (Qwen, Gemma, DeepSeek, etc.)
   - Prompt engineering (Zero-shot, Few-shot, CoT)
   - RAFT-LoRA fine-tuned models

---

## Key Features

- 🔹 Hybrid retrieval combining semantic + lexical signals  
- 🔹 Entailment-tuned retriever for logical alignment  
- 🔹 Contrastive learning with Multiple Negatives Ranking Loss (MNRL)  
- 🔹 Score-based filtering for high-quality context selection  
- 🔹 Advanced evaluation using **RePAS (Entailment, Contradiction, Coverage)**  
- 🔹 Support for multiple LLMs and prompting strategies  

---

## Dataset

- **ObliQA Dataset** (Regulatory QA)
- Custom preprocessing:
  - Document-level split (to avoid data leakage)
  - Removal of cross-document overlaps
  - Structured corpus creation

---

## Tech Stack

- **Languages:** Python  
- **Frameworks:** PyTorch, Hugging Face Transformers, SentenceTransformers  
- **Libraries:** NumPy, Pandas, BM25, NLTK  
- **Models:**  
  - LegalBERT  
  - E5 (Dense retrieval)  
  - BGE Reranker  
  - Qwen / Gemma / DeepSeek (LLMs)  

---

## Evaluation Metrics

### Retrieval
- Recall@K  
- MAP@K  
- nDCG@K  

### Generation
- **RePAS Score**
  - Entailment
  - Contradiction
  - Obligation Coverage  

---

## Results

- Significant improvement in retrieval performance using:
  - Entailment tuning  
  - Contrastive learning (MNRL)  
  - Hybrid retrieval  

- Enhanced answer quality with:
  - Retrieval-augmented prompts  
  - RAFT-LoRA fine-tuning  
