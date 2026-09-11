# Similarity Search on Employee Records using Python and Chroma DB

A hands-on lab project implementing advanced semantic similarity search, metadata filtering, and hybrid queries using **Chroma DB** and **SentenceTransformers**.

## Overview

This project demonstrates how to ingest structured records (employee profiles), convert them into rich textual representations, generate vector embeddings using SentenceTransformers (`all-MiniLM-L6-v2`), and store them within a Chroma DB collection. It provides multiple search capabilities:
1. **Semantic Similarity Search:** Finding relevant records using natural language queries (e.g., searching for Python developers or leadership roles).
2. **Metadata Filtering:** Applying hard filters based on attributes like department, experience ranges, and location.
3. **Combined Search:** Merging vector similarity search with strict metadata constraints to solve real-world talent acquisition and recommendation use cases.

## Tech Stack

- **Python 3.11+**
- **Chroma DB** (`chromadb==1.0.12`)
- **Sentence Transformers** (`sentence-transformers==4.1.0`)

## Project Structure

```text
├── similarity_employeedata.py    # Main script containing collection setup, ingestion, and search functions
└── README.md                     # Project documentation

## Setup & Installation

git clone [(https://github.com/aiwithnaveedd/similarity_search_chromadb.git)]
cd similarity_search_chromadb

pip install chromadb==1.0.12 sentence-transformers==4.1.0

python3.11 similarity_employeedata.py
