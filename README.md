
# S-RAI OS v2.6 — Policy-Governed Hybrid RAG

S-RAI OS is a browser-native, sovereign AI operating system that combines policy-driven access control with a hybrid Retrieval-Augmented Generation (RAG) engine. It runs fully client-side with no servers or external dependencies beyond the included model libraries.

---

## Features

- **Policy-Key Management**
  - Create root keys and derive agent keys
  - Enforce capabilities (`memory.write`, `rag.query`, `system.export`, etc.)
  - Audit and revoke keys

- **Hybrid RAG Engine**
  - Sparse (BM25) and dense (embedding-based) search
  - Reciprocal Rank Fusion (RRF) for result merging
  - Adjustable fusion α parameter

- **Memory Management**
  - Episodic, semantic, and procedural memory storage
  - Indexed for search and retrieval
  - Export and import memory

- **Document Ingestion**
  - Load `.txt`, `.md`, `.json`, and `.pdf` files
  - Automatic chunking for optimal RAG performance
  - Personal vs public corpus toggling

- **Identity & Sovereignty**
  - Generate DID (Decentralized Identifier)
  - Full client-side encryption for sensitive data

- **UI Features**
  - Console, results, and memory browser tabs
  - Live logs and progress indicators
  - Minimal, dark-themed, responsive design

---

## Usage

1. Open `index.html` in a modern browser.
2. Create a root policy key and derive agent keys.
3. Load documents into the personal corpus.
4. Enter a query in the Query Engine and adjust the fusion α parameter.
5. Execute RAG to retrieve and generate context-aware answers.
6. Manage memory, identities, and system state via the sidebar.

---

## Technical Stack

- Vanilla JavaScript (no backend required)
- IndexedDB for local storage
- AES-GCM encryption for sensitive data
- Xenova Transformers for embeddings and text generation
- PDF.js for PDF ingestion
- Responsive CSS with JetBrains Mono font

---

## Security & Privacy

All data and processing occur in the client browser. No external servers or APIs are required. Encryption ensures memory and corpus data remain private.

---
