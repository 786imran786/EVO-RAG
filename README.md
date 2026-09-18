# EvoRAG

**EvoRAG — An Adaptive, Self-Updating, Evidence-First RAG System**

EvoRAG is a Retrieval-Augmented Generation system designed to detect when its existing knowledge is insufficient, acquire missing information, verify it, store verified knowledge, and generate evidence-grounded answers.

> Don't know? Find out. Don't trust? Verify. Can't verify? Don't guess.

## Core Idea

Traditional RAG:

```text
User Query → Retrieve → LLM → Answer
```

EvoRAG:

```text
User Query
    ↓
Analyze
    ↓
Check Knowledge
    ↓
Detect Knowledge Gap
    ↓
Acquire Missing Knowledge
    ↓
Verify
    ↓
Ingest
    ↓
Retrieve
    ↓
Generate
    ↓
Verify Answer
```

The project focuses on adaptive knowledge acquisition, freshness, source reliability, temporal knowledge, claim-level verification, contradiction detection, and answer abstention.

## Main Components

- Query Analyzer
- Freshness Detection Engine
- Knowledge Coverage Engine
- Knowledge Gap Detector
- Dynamic Prompt Generation
- Knowledge Acquisition Engine
- Source Reliability Engine
- Claim Extraction
- Temporal Knowledge Store
- Hybrid Retrieval
- Evidence Graph
- Answer Generation
- Claim Verification Engine
- Contradiction Detection
- Self-Correction / Answer Repair

## Technology Stack

- Python
- FastAPI
- Pydantic
- AsyncIO
- Qdrant
- BM25 / Elasticsearch / OpenSearch
- Neo4j
- LLM providers
- Embedding models
- Web and API data sources

The architecture is intended to remain model- and provider-independent.

## Development Roadmap

### Phase 1 — Foundation
- Document ingestion
- Chunking
- Embeddings
- Qdrant setup
- Baseline RAG

### Phase 2 — Trust Layer
- Retrieval confidence
- Source metadata
- Citations
- Answer abstention

### Phase 3 — Adaptive Layer
- Knowledge-gap detection
- Freshness detection
- Dynamic search-query generation
- Web acquisition

### Phase 4 — Knowledge Evolution
- Temporal metadata
- Temporary and permanent knowledge
- Knowledge expiration
- Automatic updating

### Phase 5 — Verification
- Claim extraction
- Evidence matching
- Contradiction detection
- Answer repair

### Phase 6 — Intelligence Layer
- Query decomposition
- Acquisition planning
- Multi-source reasoning
- Evidence graph

### Phase 7 — Evaluation
- Hallucination benchmark
- Baseline RAG vs EvoRAG
- Accuracy and evidence coverage
- Latency and cost measurement
- Adversarial testing

### Phase 8 — Final Product
A dashboard showing:

```text
Query
 ↓
Knowledge Status
 ↓
Knowledge Gap
 ↓
Acquisition
 ↓
Sources
 ↓
Evidence
 ↓
Reasoning
 ↓
Verification
 ↓
Final Answer
```

## Research Direction

The central research question is:

> Can a RAG system dynamically acquire only the knowledge it needs instead of relying on a permanently pre-populated knowledge base?

EvoRAG aims to move RAG from simple document retrieval toward adaptive knowledge acquisition and evidence management.
