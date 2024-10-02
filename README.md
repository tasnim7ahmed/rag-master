# Mastering Retrieval-Augmented Generation with LangChain

This repository contains a comprehensive collection of Retrieval-Augmented Generation (RAG) approaches using LangChain. It demonstrates various advanced techniques for implementing RAG workflows, including indexing, retrieval, query translation, routing, and full end-to-end CRAG. The demonstrated approaches in this project solely rely on open-source embeddings and LLMs, making them suitable for local execution without the need for external services like OpenAI.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Notebooks Overview](#notebooks-overview)
- [Installation](#installation)
- [Usage](#usage)


## Features
- **Indexing**: Basic and multi-representation indexing strategies, including RAPTOR.
- **Basic Retrieval & Generation**: Examples of setting up retrieval pipelines for generating responses based on retrieved content.
- **Query Translation Approaches**: Multi-Query, RAG-Fusion, Decomposition, Step-Back Queries, HyDE (Hypothetical Document Embedding).
- **Routing**: Logical and Semantic routing mechanisms for query handling.
- **Query Construction**: Techniques for structured query generation.
- **CRAG**: Full end-to-end RAG workflows built from the ground up.
- **Open-Source Compatibility**: All embeddings and LLMs used are open-source, allowing for local execution without reliance on paid APIs.

## Notebooks Overview

### 1. LangSmithPartOne
This notebook explores the foundational concepts of **Indexing**, **Basic Retrieval and Generation**, and various **Query Translation Approaches**:
- Multi-Query
- RAG-Fusion
- Decomposition
- Step-Back Query
- HyDE
  
It also delves into **Routing** techniques, both logical and semantic, for handling diverse types of queries in RAG systems.

### 2. LangSmithPartTwo
The second notebook focuses on **Query Construction** and generating **Structured Output** from LLMs. It demonstrates how to construct queries using metadata filters and handle structured outputs for more complex scenarios.

### 3. LangSmithPartThree
This notebook addresses **advanced indexing techniques**, including:
- **Multi-representation Indexing**
- **RAPTOR**

These approaches ensure efficient document retrieval and provide flexibility in handling large datasets with various representations.

### 4. LangSmithPartFour (CRAG)
The fourth notebook provides an end-to-end **CRAG** solution. It integrates open-source embeddings, document loaders, and vector stores to create a complete RAG pipeline. This notebook emphasizes local execution using open-source tools without relying on external APIs, making it suitable for fully offline environments.

## Installation

### Prerequisites
- Python 3.8+
- Open-source LLMs and embeddings (e.g., Sentence Transformers, HuggingFace models)
- Libraries: LangChain, Chroma, Pydantic, Matplotlib

1. Clone the repository:
   ```bash
   git clone https://github.com/tasnim7ahmed/ragmaster.git
   cd ragmaster
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up environment variables if needed for tracing (optional):
   ```bash
   export LANGCHAIN_TRACING_V2="true"
   export LANGCHAIN_ENDPOINT="https://api.smith.langchain.com"
   ```

## Usage

To run each notebook:
1. Navigate to the `notebooks/` directory.
2. Start Jupyter Notebook or JupyterLab:
   ```bash
   jupyter notebook
   ```
3. Open and execute each notebook sequentially to explore the different RAG approaches.

### Example Workflow
```python
# Run the RAG chain example from LangSmithPartOne
rag_chain.invoke("How to define a RAG chain? Give me a specific code example.")
```
