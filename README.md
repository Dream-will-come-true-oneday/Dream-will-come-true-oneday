<div align="center">

# Leonardo · 杨涛华

### AI Agent Developer · Python · Agent Harness / Context Engineering / Long-horizon Workflows

<p>
  <a href="https://github.com/Dream-will-come-true-oneday"><img src="https://img.shields.io/badge/GitHub-Dream--will--come--true--oneday-181717?style=flat-square&logo=github" alt="GitHub profile" /></a>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/MCP-111827?style=flat-square" alt="MCP" />
  <img src="https://img.shields.io/badge/LangGraph-1.0-1a7f37?style=flat-square" alt="LangGraph" />
</p>

</div>

I am an undergraduate student majoring in **Network Engineering** at [Henan University](https://www.henu.edu.cn/) (Double First-Class), graduating in 2027. I am looking for opportunities in **AI Agent development**, with a focus on agent harness design, context engineering, protocol-level tool integration, and production-grade long-horizon workflows.

I enjoy turning complex model capabilities into reliable engineering systems — building agents that can plan, execute, recover, and deliver real business value. My long-term vision is **embodied intelligence**: giving Agents real hands in the physical world, so they can move from reasoning on screens to perceiving and acting in reality.

## 🧠 Professional Skills

- **Agent Harness & orchestration:** Proficient with LangGraph 1.x (SubGraph orchestration, PostgreSQL Checkpointer state persistence, interrupt approval checkpoints); understand the Framework / Harness / Runtime three-layer division of labor. Familiar with the positioning differences of OpenAI Agents SDK, Microsoft Agent Framework, and Google ADK.
- **Context engineering:** Context compression and offloading, structured handoff (goal / completed / next steps / key files / blockers / constraints), Tool Search / Schema lazy loading, token budgeting and per-task cost accounting; structured output schema design and validation.
- **Protocols & capability encapsulation:** Familiar with MCP protocol and tool dispatch, including MCP stateless core, A2A (Agent-to-Agent communication), and AG-UI (frontend event streaming). Understand Skills / SKILL.md progressive disclosure and AGENTS.md conventions.
- **Engineering & observability:** FastAPI + SSE streaming endpoints, PostgreSQL / MySQL / Redis, LangSmith full-link tracing, structlog structured logging. Familiar with OpenTelemetry GenAI semantic conventions. Git, Docker, Linux development environments.
- **Async, high availability & cost:** asyncio.gather concurrent scheduling, run_in_executor coroutinization, exponential backoff retry, circuit breaker three-state model, rate limiting. Model routing and cost optimization — shipped practice that reduced per-task cost by **40%**.
- **AI development tools:** Use Claude Code for requirement decomposition, code generation, and refactoring/debugging; experienced in AI output validation and hallucination detection.

## 💼 Internship Experience

### 🔵 ByteDance · Ocean Engine Qianchuan · Agent Development Intern

`2026.03 - 2026.07`

Built agent-powered creative analysis pipelines for livestream material production, optimizing multimodal understanding, processing throughput, and browser-side video architecture.

- **Multimodal content understanding & highlight detection:** Addressed pure-text LLM accuracy ceiling (~70%) with a three-signal weighted scoring approach — audio energy peaks (librosa), danmaku (bullet comment) heat, and Doubao 2.0 text understanding. Validated on **500+ real samples**, boosting accuracy to **90%+** and clip adoption rate from 45% to **68%**. Evaluated a frame-extraction + multimodal end-to-end approach but deferred due to per-call cost and latency; listed as a visual-model iteration direction.
- **Livestream clip pipeline parallelization:** Addressed serial processing bottlenecks (6-hour replay taking 18 minutes) by implementing concurrent Volcano ASR and Doubao LLM calls (asyncio.gather + Semaphore with concurrency limits derived from API quotas). Reduced single-task processing from 18 min to **5 min (-72%)**, with 429 rate kept below **1%**.
- **Browser-side video processing architecture refactor:** Compared WebCodecs vs FFmpeg.wasm and chose FFmpeg.wasm for Safari compatibility and muxer/demuxer implementation cost. Used WORKERFS zero-copy mounting for GB-level on-demand file reading in-browser. Reduced memory from 5GB to **50MB**; extracted 16kHz mono audio in-browser and uploaded only 30MB (from 2.5GB), completely removing server-side FFmpeg dependency.

### 🟣 MiniMax (Xiyi Technology) · Product R&D · Agent Backend Development Intern

`2025.11 - 2026.01`

Built agent tool infrastructure, long-horizon runtime reliability, and evaluation systems for production-grade LLM applications.

- **Tool invocation system:** Co-designed a Tool Registry and executor layer, unifying Schema validation, permissions, timeout/retry, circuit breaking, and critical/non-critical degradation across **23 internal tools**. Reduced parameter error rate from 9% to **1.2%**, improved call success rate to **99.2%**, and cut onboarding time for new tools from 2 weeks to **1 day**.
- **Long-horizon task runtime:** Implemented human-approval checkpoints, node-level breakpoint recovery, and resume idempotency using LangGraph interrupt + PostgreSQL Checkpointer. All **80 fault-injection scenarios** (process crash / network jitter / DB disconnect / duplicate resume) recovered successfully. Improved cross-day task completion from 87% to **98%**, and reduced breakpoint rerun cost by **67%**.
- **Evaluation & tracing:** Built node-level Trace and trajectory evaluation organized by four dimensions (result / process / efficiency / risk). Created a **500-item** golden / error-case / challenge dataset with three-level scoring (rules + LLM judge + human spot-check) and calibration of judge consistency. Bad cases feed back into the regression set; surfaced **37 issues** total, reducing diagnosis time from 2 hours to **15 minutes**.

## 🛠️ Project Experience

### [EndlessCode](https://github.com/Dream-will-come-true-oneday/EndlessCode) · Independent Development

**Intelligent terminal coding Agent** · `Python` · `MCP`

A terminal-based coding Agent supporting multiple LLM providers and MCP extensions, built around a complete loop of reasoning, tool calling, result handling, and continued action.

- **Context engineering:** Gradually compresses conversation history by session scale; triggers structured handoff (goal / completed / next steps / key files / blockers / constraints) when thresholds are exceeded. Designed a Function Calling pair validation chain to prevent result-loss exceptions, supporting hours of continuous coding without losing critical context.
- **MCP dynamic dispatch:** Built a local tool discovery index using "search-triggered + on-demand Schema injection" — a tool search / lazy loading approach. Reduced context usage by **82%** in tool libraries with hundreds of definitions, solving long-session window overflow.
- **Agent runtime security:** Multi-layer defense including sandbox-isolated execution, path normalization and boundary interception, tool-level permissions, high-risk operation HITL approval, and full-chain explainable audit — making every Agent decision path fully traceable.

## 🎓 Education

**Henan University** (Double First-Class) · Network Engineering · Undergraduate

`2023.09 - 2027.06`

## 🔭 Long-term Vision

I want to help build the bridge from **digital intelligence to physical action**. The goal is not only to make Agents better at answering questions, but to give them the perception, tools, and eventually the physical hands needed to understand and act in the real world.

<div align="center">

[GitHub](https://github.com/Dream-will-come-true-oneday) · [EndlessCode](https://github.com/Dream-will-come-true-oneday/EndlessCode) · [Email](mailto:13609048665@163.com)

<sub>Building useful agents, one tool call at a time.</sub>

</div>
