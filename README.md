<h1 align="center">Hi, I'm Govindh Kishore 👋</h1>

<h3 align="center">Math and Computing student, building retrieval systems</h3>

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

#### 🔍 [funseek](https://github.com/GovindhKishore/funseek) | [PyPI](https://pypi.org/project/funseek)
`Python` `rank-bm25` `ChromaDB` `sentence-transformers` `NetworkX`

A three-signal hybrid retrieval CLI fusing **BM25 lexical search**, **dense vector search**, and **AST-derived call-graph structural retrieval** via Reciprocal Rank Fusion.

- Evaluated across five retrieval configurations on a 30-query benchmark over ~1,260 indexed functions across scikit-learn's `model_selection`, `preprocessing`, and other subpackages
- **MRR@5: 0.6022** and **Recall@20: 0.7889** (BM25 + semantic + graph fusion) vs. **MRR@5: 0.5122**, **Recall@20: 0.7222** semantic-alone, and **MRR@5: 0.5389**, **Recall@20: 0.7389** BM25+semantic without the graph
- Implemented call-graph structural retrieval, scoring functions by call relationships to top BM25/vector results - summing decayed contributions (0.5^hop) from every reaching seed, weighted by inverse seed rank
- Identified degraded structural performance because of nodes colliding on bare function names (e.g. sklearn's repeated `fit`/`transform` across estimator classes), fixed via collision-free graph construction keying nodes on globally-unambiguous (name, class) pairs - driving the best overall fusion result (+0.063 MRR@5, +0.05 Recall@20 vs. BM25+semantic alone)
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

Relevant coursework: Object-Oriented Programming (Java), Data Structures & Algorithms, Discrete Mathematics & Graph Theory, Information Retrieval

---
