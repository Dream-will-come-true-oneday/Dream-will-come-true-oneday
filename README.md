<div align="center">

# Leonardo · 杨涛华

### AI Agent Developer · Python · Long-horizon Workflows / Agent Infrastructure

<p>
  <a href="https://github.com/Dream-will-come-true-oneday"><img src="https://img.shields.io/badge/GitHub-Dream--will--come--true--oneday-181717?style=flat-square&logo=github" alt="GitHub profile" /></a>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/MCP-111827?style=flat-square" alt="MCP" />
</p>

</div>

I am an undergraduate student majoring in **Network Engineering** at [Henan University](https://www.henu.edu.cn/) (Double First-Class), graduating in 2027. I am looking for opportunities in **AI Agent development**, with a focus on long-horizon task orchestration, tool reliability, async performance optimization, and production-grade execution.

I enjoy turning complex model capabilities into usable engineering systems — building agents that can plan, execute, recover, and deliver real business value. My long-term vision is **embodied intelligence**: giving Agents real hands in the physical world, so they can move from reasoning on screens to perceiving and acting in reality.

## 🧠 Professional Skills

- **Agent frameworks:** LangGraph (SubGraph orchestration, PostgreSQL Checkpointer state persistence, interrupt human-in-the-loop checkpoints), LangChain, Plan-and-Execute paradigm, and long-horizon task reliability design (checkpoint resume, node-level replay). Familiar with MCP protocol and tool dispatch.
- **LLM application engineering:** Prompt Engineering, Function Calling, structured output (JSON Mode / with_structured_output layered approach), and multi-model dynamic routing with cost optimization — shipped practice that reduced inference cost by 40%.
- **AI development tools:** Proficient with Claude Code for requirement decomposition, code generation, and debugging; layer Copilot line-level completion with Claude Code for complex refactoring; experienced in AI output validation and hallucination detection.
- **Async & high availability:** Deep understanding of Python async IO (asyncio.gather concurrent scheduling, run_in_executor coroutinization), exponential backoff retry, circuit breaker three-state model, and rate limiting — with hands-on multi-tool parallel performance optimization.
- **Backend & observability:** FastAPI for RESTful APIs and SSE streaming endpoints, PostgreSQL, Redis, LangSmith full-link tracing, structlog structured logging, Git, Docker, and Linux development environments.

## 💼 Internship Experience

### 🔵 ByteDance · Ocean Engine Qianchuan · Agent Development Intern

`2026.03 - 2026.07`

Built agent-powered creative analysis pipelines for livestream material production, optimizing processing throughput, detection accuracy, and video architecture at scale.

- **Livestream clip pipeline parallelization:** Addressed serial processing bottlenecks by implementing concurrent calls to Volcano ASR and Doubao LLM (asyncio.gather + Semaphore rate limiting). Reduced single-task processing time by **72%**, with 429 error rate kept below **1%** through careful API quota control.
- **Multi-signal highlight detection algorithm:** Solved pure-text LLM accuracy ceiling (~70%) with a three-signal weighted fusion approach — audio energy peaks (librosa), danmaku (bullet comment) heat, and Doubao text understanding. Boosted highlight recognition accuracy to **90%+** and user adoption rate from 45% to **68%**.
- **Browser-side video processing architecture refactor:** Rebuilt the pipeline as a pure-frontend FFmpeg.wasm architecture. Used WORKERFS virtual filesystem for zero-copy mounting, enabling GB-level on-demand file reading in the browser. Reduced memory usage to **50MB** (**-99%**); extracted audio in-browser and uploaded only 30MB, shrinking upload volume by **99%** and completely removing server-side FFmpeg dependency.

### 🟣 MiniMax (Xiyi Technology) · Product R&D · Agent Backend Development Intern

`2025.11 - 2026.01`

Built agent tool infrastructure, long-horizon runtime reliability, and evaluation systems for production-grade LLM applications.

- **Tool invocation system:** Co-designed a Tool Registry and executor layer, unifying Schema validation, permissions, timeout/retry, circuit breaking, and critical/non-critical degradation across **23 internal tools**. Reduced parameter error rate from 9% to **1.2%**, improved call success rate to **99.2%**, and cut onboarding time for new tools from 2 weeks to **1 day**.
- **Long-horizon task runtime:** Implemented human-in-the-loop checkpoints, breakpoint recovery, and resume idempotency using LangGraph interrupt + PostgreSQL Checkpointer. Achieved **100%** fault-injection recovery rate (80/80), improved cross-day task completion from 87% to **98%**, and reduced breakpoint rerun cost by **67%**.
- **Evaluation & tracing:** Built node-level Trace collection and a four-layer evaluation framework (result / process / efficiency / risk). Created a **500-item** golden / error-case / challenge dataset combining rule-based checks, LLM judges, and human spot-checking for failure attribution. Surfaced **37 regression issues**, reducing problem diagnosis time from 2 hours to **15 minutes**.

## 🛠️ Project Experience

### [EndlessCode](https://github.com/Dream-will-come-true-oneday/EndlessCode) · Independent Development

**Intelligent terminal coding Agent** · `Python` · `MCP`

A terminal-based coding Agent supporting multiple LLM providers and MCP extensions, built around a complete loop of reasoning, tool calling, result handling, and continued action.

- **Two-level context compression:** Gradually compresses conversation history by session scale; designed a Function Calling pair validation chain to prevent result-loss exceptions, supporting hours of continuous coding without losing critical context.
- **MCP dynamic dispatch:** Built a local tool discovery index with "search-triggered + Schema dynamic injection" — reducing context usage by **82%** in tool libraries with hundreds of definitions, solving long-session window overflow.
- **Five-layer security defense:** Designed a multi-layer defense system covering sandbox isolation, path filtering, and human-in-the-loop (HITL) approval, with explainable audit logs making every Agent decision fully traceable.

## 🎓 Education

**Henan University** (Double First-Class) · Network Engineering · Undergraduate

`2023.09 - 2027.06`

## 🔭 Long-term Vision

I want to help build the bridge from **digital intelligence to physical action**. The goal is not only to make Agents better at answering questions, but to give them the perception, tools, and eventually the physical hands needed to understand and act in the real world.

<div align="center">

[GitHub](https://github.com/Dream-will-come-true-oneday) · [EndlessCode](https://github.com/Dream-will-come-true-oneday/EndlessCode) · [Email](mailto:13609048665@163.com)

<sub>Building useful agents, one tool call at a time.</sub>

</div>
