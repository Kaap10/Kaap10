### [Portfolio](https://kaap10.github.io/portfolio) 
- Building AI agents, ML systems, and scalable software from idea to production
  
## >> Open Source Contributions

<details>
<summary><b><font size="+1">Apache Magpie</font></b> (<a href="https://github.com/apache/magpie"><code>apache/magpie</code></a>)</summary>

<br>

*Agent-assisted maintainership and vulnerability triage framework under the Apache Software Foundation (ASF)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Core Security HTTP Dispatcher** | Built dependency-free stdlib `urllib` engine with sandbox isolation and strict input sanitization for OSV.dev and CVE.org | [#1326](https://github.com/apache/magpie/pull/1326) |
| **Multi-Forge API Bridges** | Engineered read-only API bridges for **GitLab** and **Forgejo/Gitea** with RFC-5988 Link-header pagination | [#1369](https://github.com/apache/magpie/pull/1369), [#1441](https://github.com/apache/magpie/pull/1441), [#1469](https://github.com/apache/magpie/pull/1469) |
| **OSV.dev Vulnerability Aggregator** | Built security triage adapter querying cross-ecosystem CVE/GHSA alias graphs across 30+ package registries | [#1297](https://github.com/apache/magpie/pull/1297) |
| **LLM Token Optimization** | Reduced skill body tokens by ~20% and cut always-on system prompt frontmatter by ~50% (~350 tokens/turn saved) | [#1487](https://github.com/apache/magpie/pull/1487), [#1489](https://github.com/apache/magpie/pull/1489), [#1481](https://github.com/apache/magpie/pull/1481), [#1482](https://github.com/apache/magpie/pull/1482), [#1483](https://github.com/apache/magpie/pull/1483) |
| **AI Agent Runtime Harnesses** | Implemented runtime adapters for GitHub Copilot CLI, Aider, Goose, Ollama/vLLM (air-gapped local LLMs), and Cursor | [#1287](https://github.com/apache/magpie/pull/1287), [#1286](https://github.com/apache/magpie/pull/1286), [#1217](https://github.com/apache/magpie/pull/1217), [#1206](https://github.com/apache/magpie/pull/1206), [#1204](https://github.com/apache/magpie/pull/1204) |
| **Architecture & Governance** | Added Claude Code setup drift check mod, mod guidelines, and vendor-neutral skill descriptions | [#1552](https://github.com/apache/magpie/pull/1552), [#1541](https://github.com/apache/magpie/pull/1541), [#1550](https://github.com/apache/magpie/pull/1550) |

</details>

<details>
<summary><b><font size="+1">Microsoft PyRIT</font></b> (<a href="https://github.com/microsoft/PyRIT"><code>microsoft/PyRIT</code></a>)</summary>

<br>

*Python Risk Identification Tool for AI Red Teaming by Microsoft AI Red Team*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **GCG Attack Refactoring** | Decoupled Greedy Coordinate Gradient attack into typed modules (`CandidateProposer`, `CandidateEvaluator`, `ProgressiveScheduleController`) with VRAM-bounded tensor cleanup | [#2671](https://github.com/microsoft/PyRIT/pull/2671), [#2700](https://github.com/microsoft/PyRIT/pull/2700), [#2720](https://github.com/microsoft/PyRIT/pull/2720) (closes [#2665](https://github.com/microsoft/PyRIT/issues/2665)) |
| **Multi-Process CI Test Isolation** | Resolved MOSSBench and VLSU SQLite memory collisions in CI by enforcing isolated in-memory fixtures | [#2781](https://github.com/microsoft/PyRIT/pull/2781) (fixes [#2775](https://github.com/microsoft/PyRIT/issues/2775)) |
| **Attack Technique Factory** | Extracted dynamic reflection and cached parameter discovery in `MatrixAtomicAttackBuilder` and technique resolution | [#2879](https://github.com/microsoft/PyRIT/pull/2879), [#2795](https://github.com/microsoft/PyRIT/pull/2795) |
| **RFC 9110 HTTPTarget Byte-Length Fix** | Resolved UTF-8 byte vs character count mismatch in `Content-Length` headers, preventing payload truncation on multilingual and emoji adversarial prompts | [#3008](https://github.com/microsoft/PyRIT/pull/3008) |
| **Converter & Scorer Validation** | Added eager n-gram size validation in `ApproximateTextMatching` and disallowed empty split separators in `WordLevelConverter` | [#2911](https://github.com/microsoft/PyRIT/pull/2911), [#2912](https://github.com/microsoft/PyRIT/pull/2912) |

</details>

<details>
<summary><b><font size="+1">dynavec</font></b> (<a href="https://github.com/codeforstartups/dynavec"><code>codeforstartups/dynavec</code></a>)</summary>

<br>

*Serverless hybrid vector database & agent orchestration engine on DynamoDB + S3 Vectors*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Autonomous Agent Primitives** | Built core `ReActAgent` and step-by-step `Planner` runtimes with dynamic schema generation from `@tool` docstrings and execution budget guards | [#319](https://github.com/codeforstartups/dynavec/pull/319) |
| **Extensible Tool Registry** | Implemented thread-safe `ToolRegistry` with built-in connectors for stdlib HTTP, sandboxed Python execution, and FastMCP sessions | [#328](https://github.com/codeforstartups/dynavec/pull/328) |
| **Real-Time Token Streaming (`astream`)** | Added async SSE token streaming for OpenAI and Anthropic models with sub-50ms first-token latency | [#329](https://github.com/codeforstartups/dynavec/pull/329) |
| **Multi-Provider Chat Abstraction** | Unified OpenAI, Anthropic, and AWS Bedrock Converse APIs under a single `BaseChatModel` interface | [#317](https://github.com/codeforstartups/dynavec/pull/317) |
| **Graph Engine Resilience** | Added per-node `RetryPolicy` with exponential backoff, error fallback edges, and resumable `GraphRunState` checkpoints | [#338](https://github.com/codeforstartups/dynavec/pull/338) |
| **Hot-Tier Index Rebalancing (SPFresh)** | Implemented incremental Mini-Batch 2-Means dynamic clustering with lock-free vector migration under continuous streaming ingest | [#170](https://github.com/codeforstartups/dynavec/pull/170) |
| **Critical Graph Data Loss Fix** | Fixed bug where adding edges or linking documents inadvertently wiped existing entity types and properties | [#272](https://github.com/codeforstartups/dynavec/pull/272) (fixes [#271](https://github.com/codeforstartups/dynavec/issues/271)) |
| **HyDE & Multi-Query Expansion RFC** | Authored accepted RFC combining multi-query generation and hypothetical document embeddings via Reciprocal Rank Fusion (RRF) | [#215](https://github.com/codeforstartups/dynavec/issues/215) |
| **Offline Evaluation Suite & LLM Judge** | Shipped retrieval benchmark runner (Recall@k, MRR, nDCG) and pluggable LLM-as-a-judge for RAG faithfulness | [#185](https://github.com/codeforstartups/dynavec/pull/185), [#178](https://github.com/codeforstartups/dynavec/pull/178) |
| **MCP Server & Cost Optimization** | Created official FastMCP server for IDEs, SHA-256 chunk deduplication reducing embedding costs by 30–40%, and `py.typed` packaging | [#165](https://github.com/codeforstartups/dynavec/pull/165), [#120](https://github.com/codeforstartups/dynavec/pull/120), [#154](https://github.com/codeforstartups/dynavec/pull/154) |

</details>

<details>
<summary><b><font size="+1">SQLite Graph Memory</font></b> (<a href="https://github.com/tonydzi/sqlite-graph-memory"><code>tonydzi/sqlite-graph-memory</code></a>)</summary>

<br>

*Graph RAG on SQLite combining vector retrieval, wikilink graphs, and cross-encoder reranking*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Model Context Protocol (MCP) Server** | Implemented a pure Python stdlib JSON-RPC MCP server exposing `memory_recall` for Claude Desktop, Cursor, and Cline | [#8](https://github.com/tonydzi/sqlite-graph-memory/pull/8) (closes [#5](https://github.com/tonydzi/sqlite-graph-memory/issues/5)) |
| **Concurrency Scoping & Hygiene** | Scoped temporary answer files per call to eliminate race conditions and prevented prompt pollution by suppressing stdout fallback on 0-hit queries | [#10](https://github.com/tonydzi/sqlite-graph-memory/pull/10) (closes [#9](https://github.com/tonydzi/sqlite-graph-memory/issues/9)) |
| **Granular Error Handling via TDD** | Replaced swallowed exceptions with explicit `isError: True` diagnostics, distinguishing file I/O failures from empty recall results | [#14](https://github.com/tonydzi/sqlite-graph-memory/pull/14) (closes [#13](https://github.com/tonydzi/sqlite-graph-memory/issues/13)) |
| **Issue Diagnostics** | Reported reproducible edge cases including stdio loop crashes on non-object JSON, masked exit codes on missing indexes, and dot-file indexing | [#22](https://github.com/tonydzi/sqlite-graph-memory/issues/22), [#23](https://github.com/tonydzi/sqlite-graph-memory/issues/23), [#25](https://github.com/tonydzi/sqlite-graph-memory/issues/25) |

</details>

<details>
<summary><b><font size="+1">Layer5 Academy</font></b> (<a href="https://github.com/layer5io/layer5-academy"><code>layer5io/layer5-academy</code></a>)</summary>

<br>

*Interactive learning platform for cloud native management, service meshes, and Kubernetes*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Kind Lab Modernization** | Streamlined prerequisites, fixed broken multi-line install commands, and updated official documentation references in Kubernetes labs | [#278](https://github.com/layer5io/layer5-academy/pull/278) (closes [#277](https://github.com/layer5io/layer5-academy/issues/277)) |
| **Podman Lab Fixes** | Corrected broken static binary download URLs and updated container prerequisites | [#276](https://github.com/layer5io/layer5-academy/pull/276) (closes [#275](https://github.com/layer5io/layer5-academy/issues/275)) |
| **Observability Lab Overhaul** | Refactored Prometheus and Grafana lab setup, replacing manual binary installs with streamlined prerequisites | [#280](https://github.com/layer5io/layer5-academy/pull/280) (issue [#279](https://github.com/layer5io/layer5-academy/issues/279)) |
| **Broken Link Remediation** | Repaired dead hyperlinks and 404 targets pointing to the Meshery Playground | [#274](https://github.com/layer5io/layer5-academy/pull/274) (closes [#273](https://github.com/layer5io/layer5-academy/issues/273)) |

</details>

<details>
<summary><b><font size="+1">Meshery</font></b> (<a href="https://github.com/meshery/meshery"><code>meshery/meshery</code></a>)</summary>

<br>

*Cloud Native computing foundation management plane for infrastructure and service meshes*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Code Review & Quality Assurance** | Provided code review feedback on PR [#22030](https://github.com/meshery/meshery/pull/22030) (merged) for mobile responsive CSS selectors and parameter backward compatibility in the `extension-guide` shortcode | [#22030](https://github.com/meshery/meshery/pull/22030) |

</details>


## >> Connect with me  
[X](https://x.com/Kap10x) · [LinkedIn](https://linkedin.com/in/vardhman-gupta) · [Email](mailto:vardhmangupta2004@gmail.com) 
