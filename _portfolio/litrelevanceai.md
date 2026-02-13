---
title: "LitRelevanceAI"
excerpt: "AI tool to screen research literature relevance from Scopus exports.<br/><img src='/images/litrelevanceai-teaser.png'>"
collection: portfolio
---

### Problem
Systematic literature reviews often involve screening thousands of papers based on titles and abstracts. This process is extremely time-consuming and prone to human error, especially during the initial broad screening phase.

### Solution
**LitRelevanceAI** is a Python-based tool that leverages Large Language Models (LLMs) to automatically screen Scopus export files (CSV) for relevance. Users can define specific inclusion and exclusion criteria in natural language, and the tool evaluates each paper against these criteria.

### Key Features
*   **Automated Screening**: Processes hundreds of abstracts in minutes.
*   **Natural Language Criteria**: No complex query strings needed; just describe what you are looking for.
*   **Reasoning Logs**: The tool provide a brief justification for each inclusion/exclusion decision, ensuring transparency.
*   **Scopus Integration**: Directly supports CSV exports from Scopus.

### Tech Stack
*   **Language**: Python
*   **AI Models**: OpenAI GPT-4o / Anthropic Claude 3.5 Sonnet
*   **Data Handling**: Pandas

### Impact
Significantly reduces the manual workload in the initial stages of a systematic review, allowing researchers to focus on deep analysis of truly relevant papers.

[View on GitHub](https://github.com/Xiaotian-Liu-MKT/LitRelevanceAI)
