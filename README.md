<h1 align="center">Hi, I'm Govindh Kishore 👋</h1>

<h3 align="center">B.Sc. (Hons.) Mathematics & Computing @ BIT Mesra | Building at the intersection of Information Retrieval and LLMs</h3>

<p align="center">
  <a href="mailto:govindhkishore7@gmail.com"><img src="https://img.shields.io/badge/Email-govindhkishore7%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/govindh-kishore-2b5922323/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white" /></a>
  <a href="https://github.com/GovindhKishore"><img src="https://img.shields.io/badge/GitHub-Follow-181717?style=flat&logo=github&logoColor=white" /></a>
</p>

---

### 🧭 About Me

I'm an undergrad at **BIT Mesra** studying Mathematics and Computing, currently building **hybrid search and retrieval systems** and contributing to open-source LLM infrastructure. My work sits at the overlap of classical IR (BM25, ranking theory), dense retrieval, and applied ML systems.

- 🌱 Deep in **Information Retrieval, RAG systems**
- 🛠️ Active contributor to **[Haystack](https://github.com/deepset-ai/haystack)** - deepset's production LLM orchestration framework
- 📐 Math background (Linear Algebra, Graph Theory) directly informs how I approach retrieval and ranking problems.

---

### 🧑‍💻 Open Source - Haystack & Haystack Core Integrations

Contributing to a production Python framework for LLM orchestration and RAG.

| PR | Description |
|---|---|
| [`#11581`](https://github.com/deepset-ai/haystack/pull/11581) | Added `run_async` to `LLMEvaluator`, `FaithfulnessEvaluator`, and `ContextRelevanceEvaluator` - enables concurrent evaluation in async apps, with runtime detection of async-capable chat generators and automatic thread-pool fallback for sync-only ones |
| [`#11552`](https://github.com/deepset-ai/haystack/pull/11552) | Fixed a silent serialization bug in `LLMEvaluator.to_dict` that caused pipeline reloads to silently reset user-configured parameters |
| [`#3412`](https://github.com/deepset-ai/haystack-core-integrations/pull/3412) | Extended `GoogleGenAITextEmbedder`, `GoogleGenAIDocumentEmbedder`, and `GoogleGenAIMultimodalDocumentEmbedder` with timeout/retry support, full serialization round-trips, and test coverage |

---

### 🚀 Featured Projects

#### 🔍 [Hybrid Code Search Engine](https://github.com/GovindhKishore/codesearch)
`Python` `rank-bm25` `ChromaDB` `sentence-transformers` `NetworkX`

A three-signal hybrid retrieval CLI fusing **BM25 lexical search**, **dense vector search**, and **AST-derived call-graph structural retrieval** via Reciprocal Rank Fusion.

- Evaluated on a hand-labeled 30-query benchmark over ~1,000+ indexed functions
- **Recall@10: 0.67** (lexical + semantic fusion) vs. **0.57** semantic-alone — a +17% relative gain
- **MRR@5: 0.43**
- Implemented multi-source BFS call-graph retrieval with hop-decay scoring and a tunable structural-weight flag
- Diagnosed and documented a real node-collision bug (bare-function-name keying causing cross-class collisions, e.g. sklearn's repeated `fit`/`transform`) that degraded structural retrieval — root-caused it down to the graph construction layer
- Shipped as a production CLI: OS-native keyring for API keys, SHA-256 multi-codebase index management, mtime-based staleness detection, lazy imports cutting startup latency from ~20s to ~6s

#### 🎯 [Assessment Recommendation System](https://github.com/GovindhKishore/Assessment_Recommendation_System)
`Python` `FastAPI` `ChromaDB` `Gemini API` `Streamlit`

A modular AI backend for embedding-based recommendation over scraped product data.

- Automated scraping pipeline (BeautifulSoup) collecting 370+ product profiles
- Two-stage pipeline: candidate generation → LLM-based reranking, with fault-tolerant fallback across rate limits and provider outages
- Streamlit dashboard for real-time inspection of retrieved recommendations

---

### 🛠️ Tech Stack

**Languages:** ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Java](https://img.shields.io/badge/-Java-007396?style=flat-square&logo=openjdk&logoColor=white) ![C](https://img.shields.io/badge/-C-A8B9CC?style=flat-square&logo=c&logoColor=white)

**ML / IR:** ![scikit-learn](https://img.shields.io/badge/-scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![NumPy](https://img.shields.io/badge/-NumPy-013243?style=flat-square&logo=numpy&logoColor=white) ![pandas](https://img.shields.io/badge/-pandas-150458?style=flat-square&logo=pandas&logoColor=white)

**Backend / Infra:** ![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![ChromaDB](https://img.shields.io/badge/-ChromaDB-white?style=flat-square) ![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

**Tools:** ![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github&logoColor=white) ![PyCharm](https://img.shields.io/badge/-PyCharm-000000?style=flat-square&logo=pycharm&logoColor=white)

---

### 🎓 Education

**Birla Institute of Technology, Mesra** - B.Sc. (Hons.) Mathematics and Computing
*Expected May 2028 · CGPA: 8.46/10.0*
Relevant coursework: Object-Oriented Programming (Java), Data Structures & Algorithms, Discrete Mathematics & Graph Theory, Information Retrieval

---
