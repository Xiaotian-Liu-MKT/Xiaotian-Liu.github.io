---
title: "SearchPaperByEmbedding"
excerpt: "Semantic search tool using vector embeddings for research discovery.<br/><img src='/images/search-embedding-teaser.png'>"
collection: portfolio
---

### Problem
Traditional academic databases rely heavily on keyword matching. However, different researchers often use different terminology to describe similar concepts (e.g., "self-conscious emotions" vs. "social emotions"), leading to relevant papers being missed in literature searches.

### Solution
**SearchPaperByEmbedding** is a semantic search tool that uses vector embeddings to find research papers based on conceptual similarity rather than exact keyword matches. It transforms paper titles and abstracts into high-dimensional vectors, allowing for "fuzzy" searches that capture the underlying meaning of the research.

### Key Features
*   **Semantic Retrieval**: Finds conceptually related papers even when terminology differs.
*   **Local Vector Database**: Efficiently indexes and searches through thousands of paper embeddings.
*   **Relevance Ranking**: Ranks results based on cosine similarity to the search query.

### Tech Stack
*   **Language**: Python
*   **Embeddings**: OpenAI `text-embedding-3-small` / HuggingFace `sentence-transformers`
*   **Vector Database**: ChromaDB / FAISS

### Impact
Helps researchers discover hidden connections between different research streams and ensures a more comprehensive coverage of the literature during the discovery phase.
