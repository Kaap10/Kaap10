<div align="center">

### >> Building [Picado Labs](https://picadolabs.me/)
**Open-source, verify-first developer infrastructure for autonomous AI software engineering.**

</div>

| Project | The Problem | The Picado Edge | Contribute Now |
|---|---|---|---|
| [**build-with-ai**](https://github.com/PicadoLabs/build-with-ai) | AI coding suffers from context drift, blank-canvas paralysis, and broken code. | Zero-API CLI, 11 production templates, and persistent `.buildwithai/` memory **(1.2k+ downloads • 20+ contributors)**. | [Issues](https://github.com/PicadoLabs/build-with-ai/issues) |
| [**AI Model Router**](https://github.com/PicadoLabs/ai-model-router) | Ballooning API costs, rate limits, and unpredictable model latency. | Sub-3ms Pareto Traffic Control Room UI with Thompson Sampling RL **(3.4k+ downloads • 10+ contributors)**. | [Issues](https://github.com/PicadoLabs/ai-model-router/issues) |
| [**Terminal Agent**](https://github.com/PicadoLabs/terminal-agent) | Autonomous coding agents make unverified changes and break repository builds. | Verify-first sandboxing (Docker/psutil), 12 core tools, self-healing, and rollback **(700+ downloads • 3+ contributors)**. | [Issues](https://github.com/PicadoLabs/terminal-agent/issues) |
| [**AgentBench**](https://github.com/PicadoLabs/agent-bench) | Existing benchmarks test isolated toy prompts rather than multi-turn agents on codebases. | 12 polyglot benchmarks, local Ollama mode ($0 cost), GitHub PR ingestion, and 5D scoring **(3+ contributors)**. | [Issues](https://github.com/PicadoLabs/agent-bench/issues) |

<div align="center">

</div>


## >> Open Source Contributions
</div align="center">
<details>
<summary><img src="https://github.com/apache.png?size=40" width="18" height="18" alt="Apache" /> <b><font size="+1">Apache Magpie</font></b></summary>

<br>

*Agent-assisted maintainership and vulnerability triage framework under the Apache Software Foundation (ASF) — [`apache/magpie`](https://github.com/apache/magpie)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Core Security HTTP Dispatcher** | Built dependency-free stdlib `urllib` engine with sandbox isolation and strict input sanitization for OSV.dev and CVE.org | [#1326](https://github.com/apache/magpie/pull/1326) |
| **Multi-Forge API Bridges** | Engineered read-only API bridges for **GitLab** and **Forgejo/Gitea** with RFC-5988 Link-header pagination | [#1369](https://github.com/apache/magpie/pull/1369), [#1441](https://github.com/apache/magpie/pull/1441), [#1469](https://github.com/apache/magpie/pull/1469) |
| **OSV.dev Vulnerability Aggregator** | Built security triage adapter querying cross-ecosystem CVE/GHSA alias graphs across 30+ package registries | [#1297](https://github.com/apache/magpie/pull/1297) |
| **Agent Guard Plugin Discovery** | Fixed `agent-guard` dispatcher to discover contributed skill guards nested under `plugins/*/skills/*/guards`, restoring pre-execution security enforcement across plugin skills | [#1757](https://github.com/apache/magpie/pull/1757) (closes [#1756](https://github.com/apache/magpie/issues/1756)) |
| **Public-Surface Security Embargo Scrub** | Built zero-token deterministic Claude Code mod hook intercepting git and gh CLI calls to prevent security embargo leaks on public surfaces (CVE references, vulnerability classes) with fail-closed safeguards | [#1676](https://github.com/apache/magpie/pull/1676) (part of [#1497](https://github.com/apache/magpie/issues/1497)) |
| **Zero-Token Claude Code CLI Mods** | Implemented zero-token `/magpie-status` and `/magpie-skills` Claude Code mod commands, setup drift check, and architecture guidelines | [#1601](https://github.com/apache/magpie/pull/1601), [#1667](https://github.com/apache/magpie/pull/1667), [#1552](https://github.com/apache/magpie/pull/1552), [#1541](https://github.com/apache/magpie/pull/1541), [#1550](https://github.com/apache/magpie/pull/1550) |
| **AI Agent Runtime Harnesses** | Implemented runtime adapters and guides for GitHub Copilot CLI, Aider, Goose, Ollama/vLLM (air-gapped local LLMs), and Cursor | [#1287](https://github.com/apache/magpie/pull/1287), [#1286](https://github.com/apache/magpie/pull/1286), [#1217](https://github.com/apache/magpie/pull/1217), [#1206](https://github.com/apache/magpie/pull/1206), [#1204](https://github.com/apache/magpie/pull/1204) |
| **CI Multi-Batch Test Normalization** | Supported stdin `-` and normalized Windows path separators in `ci-pytest-batches.py`, resolving silent test drops on cross-platform CI pipelines | [#1767](https://github.com/apache/magpie/pull/1767) (closes [#1766](https://github.com/apache/magpie/issues/1766)) |
| **Setup Doctor Probe Memory Caching** | Held diagnostic doctor probe 3 and 5 outputs in memory with regression tests to prevent repeated subprocess re-probing | [#1776](https://github.com/apache/magpie/pull/1776) (closes [#1775](https://github.com/apache/magpie/issues/1775)) |
| **LLM Token Optimization** | Reduced skill body tokens by ~20% and cut always-on system prompt frontmatter by ~50% (~350 tokens/turn saved) across contributor growth skills | [#1487](https://github.com/apache/magpie/pull/1487), [#1489](https://github.com/apache/magpie/pull/1489), [#1481](https://github.com/apache/magpie/pull/1481), [#1482](https://github.com/apache/magpie/pull/1482), [#1483](https://github.com/apache/magpie/pull/1483) |
| **Code Review & Quality Assurance** | Conducted architectural and security code reviews on Discourse bridge transport security boundaries ([#1755](https://github.com/apache/magpie/pull/1755)), triage staleness prompt fixes ([#1753](https://github.com/apache/magpie/pull/1753)), transient retry backoff ([#1752](https://github.com/apache/magpie/pull/1752)), Bitbucket approval writes ([#1746](https://github.com/apache/magpie/pull/1746)), CI workspace test failure enforcement ([#1807](https://github.com/apache/magpie/pull/1807)), and local archive read boundaries ([#1811](https://github.com/apache/magpie/pull/1811)) | [#1755](https://github.com/apache/magpie/pull/1755), [#1753](https://github.com/apache/magpie/pull/1753), [#1752](https://github.com/apache/magpie/pull/1752), [#1746](https://github.com/apache/magpie/pull/1746), [#1807](https://github.com/apache/magpie/pull/1807), [#1811](https://github.com/apache/magpie/pull/1811), [#1701](https://github.com/apache/magpie/pull/1701), [#1673](https://github.com/apache/magpie/pull/1673) |
| **First-Run Setup Guides & CLI Robustness** | Added welcome onboarding guides for contributor-growth and utilities families, and fixed non-interactive TTY crashes in Vulnogram setup | [#1702](https://github.com/apache/magpie/pull/1702), [#1669](https://github.com/apache/magpie/pull/1669), [#1742](https://github.com/apache/magpie/pull/1742) |

</details>

<details>
<summary><img src="https://github.com/microsoft.png?size=40" width="18" height="18" alt="Microsoft" /> <b><font size="+1">Microsoft PyRIT</font></b></summary>

<br>

*Python Risk Identification Tool for AI Red Teaming by Microsoft AI Red Team — [`microsoft/PyRIT`](https://github.com/microsoft/PyRIT)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **GCG Attack Refactoring** | Decoupled Greedy Coordinate Gradient attack into typed modules (`CandidateProposer`, `CandidateEvaluator`, `ProgressiveScheduleController`) with VRAM-bounded tensor cleanup | [#2671](https://github.com/microsoft/PyRIT/pull/2671), [#2700](https://github.com/microsoft/PyRIT/pull/2700), [#2720](https://github.com/microsoft/PyRIT/pull/2720) (closes [#2665](https://github.com/microsoft/PyRIT/issues/2665)) |
| **Modern LLM Chat Template Injection Detection** | Extended `StaticPromptInjectionScorer` to detect control and turn delimiter tokens across Meta Llama 3 (`<\|start_header_id\|>`, `<\|eot_id\|>`), Google Gemma (`<start_of_turn>`, `<end_of_turn>`), and Microsoft Phi-3/4 (`<\|end\|>`) | [#3484](https://github.com/microsoft/PyRIT/pull/3484) (fixes [#3483](https://github.com/microsoft/PyRIT/issues/3483)) |
| **XSS Executable Data URI Detection** | Expanded `XSSOutputScorer` to detect executable and script-bearing data URIs across SVG (`image/svg+xml`) and JavaScript MIME types (`text/javascript`, `application/javascript`, `application/x-javascript`, `text/ecmascript`) across HTML tags, markdown links/images, and form actions with strict boundary safeguards | [#3400](https://github.com/microsoft/PyRIT/pull/3400) (closes [#3399](https://github.com/microsoft/PyRIT/issues/3399)) |
| **AI & Cloud Credential Leak Detection** | Added detection patterns for OpenAI, Anthropic, and Hugging Face API keys as well as modern GitHub fine-grained PATs (`github_pat_`) in `CredentialLeakScorer` | [#3286](https://github.com/microsoft/PyRIT/pull/3286), [#3236](https://github.com/microsoft/PyRIT/pull/3236) (closes [#3285](https://github.com/microsoft/PyRIT/issues/3285), [#3235](https://github.com/microsoft/PyRIT/issues/3235)) |
| **Piped Shell & Azure Exfiltration Detection** | Expanded `ShellCommandOutputScorer` to detect piped execution across modern shells (`zsh`, `dash`, PowerShell, `pwsh`, `iex`) and Azure CLI / environment exfiltration patterns | [#3308](https://github.com/microsoft/PyRIT/pull/3308) (closes [#3307](https://github.com/microsoft/PyRIT/issues/3307)) |
| **Windows Canonical Path Traversal Scorer** | Added canonical Windows proof-of-concept targets `win.ini` and IIS `web.config` with URL-encoded dot handling and strict file-end boundary validation in `PathTraversalOutputScorer` | [#3488](https://github.com/microsoft/PyRIT/pull/3488) (fixes [#3487](https://github.com/microsoft/PyRIT/issues/3487)) |
| **Adversarial Scorer Bypass Fixes** | Extended `SSRFOutputScorer` to detect full `127.0.0.0/8` loopback block; eliminated comment syntax bypasses in `SQLInjectionOutputScorer`; and added `user:password` and IPv4 support to `OpenRedirectOutputScorer` | [#3234](https://github.com/microsoft/PyRIT/pull/3234), [#3230](https://github.com/microsoft/PyRIT/pull/3230), [#3260](https://github.com/microsoft/PyRIT/pull/3260) (closes [#3233](https://github.com/microsoft/PyRIT/issues/3233), [#3204](https://github.com/microsoft/PyRIT/issues/3204), [#3259](https://github.com/microsoft/PyRIT/issues/3259)) |
| **URL Evasion Path Encoding** | Added configurable `safe` parameter to `UrlConverter` with default `safe=""` to enforce complete URL encoding of reserved characters including forward slashes (`/` -> `%2F`), ensuring path traversal and SSRF adversarial payloads are properly encoded for evasion testing | [#3402](https://github.com/microsoft/PyRIT/pull/3402) (closes [#3401](https://github.com/microsoft/PyRIT/issues/3401)) |
| **RFC 9110 HTTPTarget Byte-Length Fix** | Stripped hop-by-hop framing headers (`Transfer-Encoding` & `Content-Length`) in `HTTPTarget`, preventing payload truncation on multilingual and emoji adversarial prompts | [#3008](https://github.com/microsoft/PyRIT/pull/3008) |
| **Attack Technique Factory** | Extracted dynamic reflection and cached parameter discovery in `MatrixAtomicAttackBuilder` and technique resolution | [#2879](https://github.com/microsoft/PyRIT/pull/2879), [#2795](https://github.com/microsoft/PyRIT/pull/2795) (closes [#2869](https://github.com/microsoft/PyRIT/issues/2869)) |
| **Multi-Process CI Test Isolation** | Resolved MOSSBench and VLSU SQLite memory collisions in CI by enforcing isolated in-memory fixtures | [#2781](https://github.com/microsoft/PyRIT/pull/2781) (fixes [#2775](https://github.com/microsoft/PyRIT/issues/2775)) |
| **Image Converter CMYK Fix** | Handled CMYK color mode conversion in `BaseImageToImageConverter` and `ImageCompressionConverter` when output format is PNG, preventing `OSError` crashes | [#3258](https://github.com/microsoft/PyRIT/pull/3258) (closes [#3257](https://github.com/microsoft/PyRIT/issues/3257)) |
| **Converter & Scorer Validation** | Added eager n-gram size validation in `ApproximateTextMatching` and disallowed empty split separators in `WordLevelConverter` | [#2911](https://github.com/microsoft/PyRIT/pull/2911), [#2912](https://github.com/microsoft/PyRIT/pull/2912) |

</details>

<details>
<summary><img src="https://github.com/codeforstartups.png?size=40" width="18" height="18" alt="Dynavec" /> <b><font size="+1">dynavec</font></b></summary>

<br>

*Serverless hybrid vector database & agent orchestration engine on DynamoDB + S3 Vectors — [`codeforstartups/dynavec`](https://github.com/codeforstartups/dynavec)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Autonomous Agent Primitives** | Built core `ReActAgent` and step-by-step `Planner` runtimes with dynamic schema generation from `@tool` docstrings and execution budget guards | [#319](https://github.com/codeforstartups/dynavec/pull/319) |
| **Extensible Tool Registry** | Implemented thread-safe `ToolRegistry` with built-in connectors for stdlib HTTP, sandboxed Python execution, and FastMCP sessions | [#328](https://github.com/codeforstartups/dynavec/pull/328) |
| **Real-Time Token Streaming (`astream`)** | Added async SSE token streaming for OpenAI and Anthropic models with sub-50ms first-token latency | [#329](https://github.com/codeforstartups/dynavec/pull/329) |
| **Multi-Provider Chat Abstraction** | Unified OpenAI, Anthropic, and AWS Bedrock Converse APIs under a single `BaseChatModel` interface | [#317](https://github.com/codeforstartups/dynavec/pull/317) |
| **Graph Engine Resilience** | Added per-node `RetryPolicy` with exponential backoff, error fallback edges, and resumable `GraphRunState` checkpoints | [#338](https://github.com/codeforstartups/dynavec/pull/338) |
| **Hot-Tier Index Rebalancing (SPFresh)** | Implemented incremental Mini-Batch 2-Means dynamic clustering with lock-free vector migration under continuous streaming ingest | [#170](https://github.com/codeforstartups/dynavec/pull/170) |
| **Critical Graph Data Loss Fix** | Fixed bug where adding edges or linking documents inadvertently wiped existing entity types and properties | [#272](https://github.com/codeforstartups/dynavec/pull/272) (fixes [#271](https://github.com/codeforstartups/dynavec/issues/271)) |
| **OpenAI Assistants & MCP Integration** | Added OpenAI Assistants `file_search` tool adapter, official FastMCP server for IDEs, and SHA-256 chunk deduplication reducing embedding costs by 30–40% | [#214](https://github.com/codeforstartups/dynavec/pull/214), [#165](https://github.com/codeforstartups/dynavec/pull/165), [#120](https://github.com/codeforstartups/dynavec/pull/120), [#154](https://github.com/codeforstartups/dynavec/pull/154) |
| **HyDE & Multi-Query Expansion RFC** | Authored accepted RFC combining multi-query generation and hypothetical document embeddings via Reciprocal Rank Fusion (RRF) | [#215](https://github.com/codeforstartups/dynavec/issues/215) |
| **Offline Evaluation Suite & LLM Judge** | Shipped retrieval benchmark runner (Recall@k, MRR, nDCG) and pluggable LLM-as-a-judge for RAG faithfulness | [#185](https://github.com/codeforstartups/dynavec/pull/185), [#178](https://github.com/codeforstartups/dynavec/pull/178) |
| **Collaborator Code Review & AWS Diagnostics** | Reviewed and approved S3 Vectors client error translation ([#346](https://github.com/codeforstartups/dynavec/pull/346)) and built `aws doctor` CLI command auditing IAM permissions, credentials, and endpoint latencies ([#144](https://github.com/codeforstartups/dynavec/pull/144)) | [#346](https://github.com/codeforstartups/dynavec/pull/346), [#144](https://github.com/codeforstartups/dynavec/pull/144) |

</details>

<details>
<summary><img src="https://github.com/tonydzi.png?size=40" width="18" height="18" alt="SQLite Graph Memory" /> <b><font size="+1">SQLite Graph Memory</font></b></summary>

<br>

*Graph RAG on SQLite combining vector retrieval, wikilink graphs, and cross-encoder reranking — [`tonydzi/sqlite-graph-memory`](https://github.com/tonydzi/sqlite-graph-memory)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Model Context Protocol (MCP) Server** | Implemented a pure Python stdlib JSON-RPC MCP server exposing `memory_recall` for Claude Desktop, Cursor, and Cline | [#8](https://github.com/tonydzi/sqlite-graph-memory/pull/8) (closes [#5](https://github.com/tonydzi/sqlite-graph-memory/issues/5)) |
| **Stdio Loop Fault Tolerance** | Guarded stdio JSON-RPC loop against unhandled non-object JSON payloads (e.g., bare literals, arrays), returning structured `-32600 Invalid Request` responses without crashing the server process | [#32](https://github.com/tonydzi/sqlite-graph-memory/pull/32) (closes [#22](https://github.com/tonydzi/sqlite-graph-memory/issues/22)) |
| **Source Execution & Child Process Resolution** | Resolved sibling script execution and injected `src/` into child `PYTHONPATH` so the MCP server executes directly from source checkouts without requiring package pre-installation, and propagated non-zero exit codes in `--test` mode | [#33](https://github.com/tonydzi/sqlite-graph-memory/pull/33) (closes [#24](https://github.com/tonydzi/sqlite-graph-memory/issues/24)) |
| **Concurrency Scoping & Hygiene** | Scoped temporary answer files per call to eliminate race conditions and prevented prompt pollution by suppressing stdout fallback on 0-hit queries | [#10](https://github.com/tonydzi/sqlite-graph-memory/pull/10) (closes [#9](https://github.com/tonydzi/sqlite-graph-memory/issues/9)) |
| **Granular Error Handling via TDD** | Replaced swallowed exceptions with explicit `isError: True` diagnostics, distinguishing file I/O failures from empty recall results | [#14](https://github.com/tonydzi/sqlite-graph-memory/pull/14) (closes [#13](https://github.com/tonydzi/sqlite-graph-memory/issues/13)) |
| **Code Reviews & Release Verification** | Reviewed and approved v0.3.1 release with macOS indexing fix and dynamic version assert ([#27](https://github.com/tonydzi/sqlite-graph-memory/pull/27)), dot-file indexing skip ([#36](https://github.com/tonydzi/sqlite-graph-memory/pull/36)), and relative index cwd resolution ([#48](https://github.com/tonydzi/sqlite-graph-memory/pull/48)) | [#27](https://github.com/tonydzi/sqlite-graph-memory/pull/27), [#36](https://github.com/tonydzi/sqlite-graph-memory/pull/36), [#48](https://github.com/tonydzi/sqlite-graph-memory/pull/48)) |
| **Issue Diagnostics** | Reported reproducible regressions including dot-file indexing in note ingestion and masked exit codes on missing embedding indexes | [#25](https://github.com/tonydzi/sqlite-graph-memory/issues/25), [#23](https://github.com/tonydzi/sqlite-graph-memory/issues/23) |

</details>

<details>
<summary><b><font size="+1">Other Organisations</font></b></summary>
<br>

<details>
<summary><img src="https://github.com/apache.png?size=40" width="18" height="18" alt="Apache Airflow" /> <b><font size="+1">Apache Airflow</font></b></summary>

<br>

*Platform to programmatically author, schedule, and monitor workflows under the Apache Software Foundation (ASF) — [`apache/airflow`](https://github.com/apache/airflow)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Task State Store Route Exception Translation** | Implemented domain-to-HTTP exception translation in `PATCH` Task State Store route, preventing unhandled domain `ValueError` crashes and mapping them cleanly to `HTTPException(404)` with complete autospec unit tests | [#73753](https://github.com/apache/airflow/pull/73753) |
| **Asset State Store Route Exception Translation** | Translated domain-level `ValueError`s in Asset State Store routes to `HTTPException(400)`, preventing internal server traces from leaking on invalid client requests | [#74179](https://github.com/apache/airflow/pull/74179) |
| **Task State Store Test Suite Refinement** | Refined docstrings and strengthened assertion details across FastAPI Task State Store test suites | [#73939](https://github.com/apache/airflow/pull/73939) |

</details>

<details>
<summary><img src="https://github.com/microsoft.png?size=40" width="18" height="18" alt="Microsoft AGT" /> <b><font size="+1">Microsoft Agent Governance Toolkit</font></b></summary>

<br>

*Policy enforcement, zero-trust identity, execution sandboxing, and reliability engineering for autonomous AI agents covering OWASP Agentic Top 10 — [`microsoft/agent-governance-toolkit`](https://github.com/microsoft/agent-governance-toolkit)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Hypervisor Workspace Isolation Hardening** | Fixed critical path traversal (`..`) escapes and sibling directory prefix collisions (`session-1` vs `session-10`) in `SessionScope.is_path_allowed`, enforcing strict canonical boundary checks and rejecting traversal identifiers in cross-session access grants | [#4356](https://github.com/microsoft/agent-governance-toolkit/pull/4356) (fixes [#4355](https://github.com/microsoft/agent-governance-toolkit/issues/4355)) |
| **Hypervisor Boundary Vulnerability Disclosure** | Identified and documented traversal vulnerabilities in agent hypervisor session scoping with reproduction test cases | [#4355](https://github.com/microsoft/agent-governance-toolkit/issues/4355) |

</details>

<details>
<summary><img src="https://github.com/meshery.png?size=40" width="18" height="18" alt="Meshery" /> <b><font size="+1">Meshery</font></b></summary>

<br>

*Cloud Native computing foundation management plane for infrastructure and service meshes — [`meshery/meshery`](https://github.com/meshery/meshery)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Code Review & Quality Assurance** | Provided code review feedback on PR [#22030](https://github.com/meshery/meshery/pull/22030) (merged), verifying responsive layout fixes and catching trailing newline and CSS bracket formatting nits in `extension-guide.html` and `edges-guide.md` | [#22030](https://github.com/meshery/meshery/pull/22030) |

</details>

<details>
<summary><img src="https://github.com/layer5io.png?size=40" width="18" height="18" alt="Layer5" /> <b><font size="+1">Layer5 Academy</font></b></summary>

<br>

*Interactive learning platform for cloud native management, service meshes, and Kubernetes — [`layer5io/layer5-academy`](https://github.com/layer5io/layer5-academy)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Kind Lab Modernization** | Streamlined prerequisites, fixed broken multi-line install commands, and updated official documentation references in Kubernetes labs | [#278](https://github.com/layer5io/layer5-academy/pull/278) (closes [#277](https://github.com/layer5io/layer5-academy/issues/277)) |
| **Podman Lab Fixes** | Corrected broken static binary download URLs and updated container prerequisites | [#276](https://github.com/layer5io/layer5-academy/pull/276) (closes [#275](https://github.com/layer5io/layer5-academy/issues/275)) |
| **Observability Lab Overhaul** | Refactored Prometheus and Grafana lab setup, replacing manual binary installs with streamlined prerequisites | [#280](https://github.com/layer5io/layer5-academy/pull/280) (issue [#279](https://github.com/layer5io/layer5-academy/issues/279)) |
| **Broken Link Remediation** | Repaired dead hyperlinks and 404 targets pointing to the Meshery Playground | [#274](https://github.com/layer5io/layer5-academy/pull/274) (closes [#273](https://github.com/layer5io/layer5-academy/issues/273)) |

</details>

<details>
<summary><img src="https://github.com/meshery-extensions.png?size=40" width="18" height="18" alt="TCS Labs" /> <b><font size="+1">TCS Labs Academy</font></b></summary>

<br>

*Meshery enterprise learning labs and cloud-native service mesh tracks for TCS Labs — [`meshery-extensions/tcslabs-academy`](https://github.com/meshery-extensions/tcslabs-academy)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Service Mesh Performance Documentation Fix** | Updated outdated SMP orientation links to the canonical specification authority at `smp-spec.io` | [#70](https://github.com/meshery-extensions/tcslabs-academy/pull/70) (fixes [#69](https://github.com/meshery-extensions/tcslabs-academy/issues/69)) |

</details>

<details>
<summary><img src="https://github.com/phasespace-labs.png?size=40" width="18" height="18" alt="Palinode" /> <b><font size="+1">Palinode</font></b></summary>

<br>

*Memory substrate for AI agents and developer tools — Git-versioned, file-native, and MCP-first — [`phasespace-labs/palinode`](https://github.com/phasespace-labs/palinode)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **POSIX Relative Path Normalization** | Normalized `to_rel_path()` in `path_guard` to enforce POSIX forward slashes (`/`) across Windows runtimes, eliminating backslash leakage across MCP tool outputs and resolving associative memory search failures | [#228](https://github.com/phasespace-labs/palinode/pull/228) (closes [#214](https://github.com/phasespace-labs/palinode/issues/214)) |
| **Non-Signalling Win32 Process Probe** | Replaced signalling `os.kill(pid, 0)` with Win32 `OpenProcess` & `WaitForSingleObject` to probe worker process liveness on Windows without interrupting console process groups | [#215](https://github.com/phasespace-labs/palinode/pull/215) (fixes [#212](https://github.com/phasespace-labs/palinode/issues/212)) |
| **Diagnostics Surface Hardening & AST Guard** | Cleaned up bare issue references across diagnostic health modules and implemented automated AST test guard preventing private issue numbers from leaking to user surfaces | [#207](https://github.com/phasespace-labs/palinode/pull/207) (fixes [#205](https://github.com/phasespace-labs/palinode/issues/205)) |

</details>

<details>
<summary><img src="https://github.com/vllm-project.png?size=40" width="18" height="18" alt="vLLM" /> <b><font size="+1">Semantic Router</font></b></summary>

<br>

*Open, programmable decision layer and dynamic semantic router for LLMs and compute clusters under vLLM — [`vllm-project/semantic-router`](https://github.com/vllm-project/semantic-router)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Explicit UTF-8 Encoding for Config Pipeline** | Enforced explicit `encoding="utf-8"` across CLI configuration operations and runtime loaders, eliminating `UnicodeDecodeError` crashes on Windows and non-UTF-8 locale systems | [#5339](https://github.com/vllm-project/semantic-router/pull/5339) (closes [#5324](https://github.com/vllm-project/semantic-router/issues/5324)) |
| **Multi-Model Shadowing & Collision Report** | Discovered and documented architectural bug where multi-model runtimes silently shadow colliding model definitions when names are omitted, causing corrupted health status tracking | [#5347](https://github.com/vllm-project/semantic-router/issues/5347) |
| **CLI Locale Encoding Regression Report** | Identified and documented platform-specific encoding crash in configuration file parser under non-UTF-8 environments | [#5324](https://github.com/vllm-project/semantic-router/issues/5324) |

</details>

<details>
<summary><img src="https://github.com/pangular-inspector.png?size=40" width="18" height="18" alt="Angular DevTools" /> <b><font size="+1">Angular DevTools</font></b></summary>

<br>

*Inspection and diagnostics toolsuite for Angular components, signals, DI, and routing across browser extensions and MCP agent environments — [`pangular-inspector/devtools`](https://github.com/pangular-inspector/devtools)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **MCP Agent Clear-Recordings Tool** | Added `clear-recordings` agent tool to reset recorded HTTP calls, router navigations, and Analog server calls between reproduction runs, with action-level gating and panel event broadcast | [#365](https://github.com/pangular-inspector/devtools/pull/365) |
| **Component Tree Hierarchy Traversal** | Fixed DOM traversal bug in `walkAngularTree()` that aborted recursion on non-component host elements, restoring missing child components nested inside standard HTML wrappers (`<div>`, `<section>`, `<main>`) | [#12](https://github.com/pangular-inspector/devtools/pull/12) (closes [#11](https://github.com/pangular-inspector/devtools/issues/11)) |
| **Route Metadata & Redirect Inspector** | Enhanced route extraction RPC scanner and Route Inspector UI to parse and display `redirectTo` targets, route titles, and metadata across static string and dynamic resolver declarations | [#10](https://github.com/pangular-inspector/devtools/pull/10) (closes [#9](https://github.com/pangular-inspector/devtools/issues/9)) |
| **Configurable Lint Rule Enforcement** | Added public configuration option `lint: { rules: { [ruleName]: false } }` allowing granular rule disabling across AST template, pipe, form, route, and Analog checks in devtools, agent tools, and CI CLI exports | [#439](https://github.com/pangular-inspector/devtools/pull/439) (merged via [#440](https://github.com/pangular-inspector/devtools/pull/440)) |

</details>

<details>
<summary><img src="https://github.com/santoshyadavdev.png?size=40" width="18" height="18" alt="Monorepo Doctor" /> <b><font size="+1">Monorepo Doctor</font></b></summary>

<br>

*AI agent skill that audits JS/TS monorepos for package boundaries, circular dependencies, caching, and CI test coverage — [`santoshyadavdev/monorepo-doctor`](https://github.com/santoshyadavdev/monorepo-doctor)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Scanner Runtime Dependency Preservation** | Fixed bug where mixed default runtime imports with named type specifiers (e.g., `import Button, { type ButtonProps } from '@acme/ui'`) were discarded as type-only, eliminating false negatives in circular dependency detection, boundary checks, and undeclared workspace dependencies | [#4](https://github.com/santoshyadavdev/monorepo-doctor/pull/4) (fixes [#3](https://github.com/santoshyadavdev/monorepo-doctor/issues/3)) |

</details>

<details>
<summary><img src="https://github.com/PhilanthroPy-Project.png?size=40" width="18" height="18" alt="PhilanthroPy" /> <b><font size="+1">PhilanthroPy</font></b></summary>

<br>

*scikit-learn–native predictive analytics library for nonprofit fundraising, donor propensity, and revenue forecasting — [`PhilanthroPy-Project/PhilanthroPy`](https://github.com/PhilanthroPy-Project/PhilanthroPy)*

| Contribution | Impact & Key Highlights | Reference |
| :--- | :--- | :--- |
| **Transformer Timezone Validation Guard** | Added unit test suite in `EncounterRecencyTransformer` guarding against invalid timezone names, ensuring accurate `KeyError` exceptions are raised instead of misleading tz-aware warnings | [#221](https://github.com/PhilanthroPy-Project/PhilanthroPy/pull/221) (closes [#204](https://github.com/PhilanthroPy-Project/PhilanthroPy/issues/204)) |

</details>

<details>
<summary> <b><font size="+1">All Contributions</font></b></summary>

| Contribution | Reference |
| :--- | :--- |
| **All Merged PRs** | [View All Merged PRs](https://github.com/search?q=is%3Apr+is%3Amerged+author%3AKaap10&type=pullrequests) |
| **Issues Authored** | [View All Authored Issues](https://github.com/search?q=is%3Aissue+author%3AKaap10&type=issues) |

</details>

</details>

</div>

---

<div align="center">

### >> <u>Connect</u> with me  
[X](https://x.com/Kap10x) · [LinkedIn](https://linkedin.com/in/vardhman-gupta) · [Email](mailto:vardhmangupta2004@gmail.com) · [Portfolio](https://kaap10.github.io/portfolio) · [Blogs](https://kaap10.github.io/blogs/intro)   

</div>

