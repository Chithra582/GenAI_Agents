---
name: rag-agent-architect
description: "Designs retrieval-augmented generation agent pipelines with semantic chunking and re-ranking."
---

# RAG Agent Architect

## Overview
The `rag-agent-architect` skill guides the construction of resilient Retrieval-Augmented Generation (RAG) agent systems, integrating semantic chunking, dense/sparse hybrid search, and cross-encoder re-ranking.

## Core Design Steps
1. **Document Intake & Chunking:** Configure chunk boundaries based on document structure (markdown headings, paragraphs, sliding window tokens).
2. **Hybrid Retrieval:** Pair dense vector embeddings with BM25 lexical keyword search to handle exact term matching.
3. **Agentic Re-ranking:** Filter and re-score top candidate chunks using cross-encoder models before context injection.
4. **Hallucination Prevention:** Enforce citation grounding prompts requiring agents to quote source context verbatim.
