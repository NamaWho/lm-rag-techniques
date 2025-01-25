# Question-Answering System with Retrieval-Augmented Generation (RAG)

## Overview
This project implements and evaluates a **Question-Answering (QA) system** powered by **Retrieval-Augmented Generation (RAG)**. It has been conducted by: L. Arduini, D. N. Ghaneh, L. Menchini, C. Petruzzella. The primary goal is to integrate and assess advanced document retrieval methods combined with large language models (LLMs) to generate accurate, context-aware responses for user queries. The system leverages methods such as **Rank Fusion** and **Cascading Retrieval** for optimized document retrieval and contextual QA generation.

## Key Features
- **Document Retrieval**:
  - Sparse Retrieval: BM25 for term-based matching.
  - Dense Retrieval: Embedding-based semantic similarity.
  - Rank Fusion: Combining sparse and dense retrieval scores.
  - Cascading Retrieval: Utilizing cross-encoders and rerankers.
- **Question-Answering**:
  - Context-aware response generation using a state-of-the-art LLM (Llama 3.2-1B).
- **Evaluation Framework**:
  - Quantitative metrics: NDCG, Recall.
  - Human-centric evaluation: Scoring responses from 0 (irrelevant) to 2 (highly relevant) with motivations for scores.

## Dataset
- **TREC-COVID**: A real-world dataset simulating medical information retrieval challenges.

## Usage
1. Load and preprocess the TREC-COVID dataset.
2. Configure retrieval strategies (BM25, dense retrieval, etc.).
3. Generate responses using the Llama 3.2-1B model with retrieved documents as context.
4. Evaluate responses with metrics (NDCG, Recall) and human annotations.

## Technologies Used
- **Python Libraries**: Sentence Transformers, Rank BM25, PyTrecEval, HuggingFace Transformers.
- **Model**: Llama 3.2-1B for language generation.
- **Dataset**: TREC-COVID.

## Structure
- **Document Retrieval**: Evaluate sparse, dense, and hybrid methods.
- **QA Generation**: Generate high-quality, context-aware responses.
- **Evaluation**: Score and annotate responses with human judgments.

## Contributing
We welcome contributions! Follow these steps:
1. Fork this repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit changes and open a Pull Request.

## License
This project is licensed under the [MIT License](LICENSE).

---
Feel free to reach out for any questions or feedback!
