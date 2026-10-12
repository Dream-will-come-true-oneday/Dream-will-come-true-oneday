<div align="center">

# Leonardo · 杨涛华

### AI Agent Developer · Python · Long-horizon Workflows / Agent Infrastructure

<p>
  <a href="https://github.com/Dream-will-come-true-oneday"><img src="https://img.shields.io/badge/GitHub-Dream--will--come--true--oneday-181717?style=flat-square&logo=github" alt="GitHub profile" /></a>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/MCP-111827?style=flat-square" alt="MCP" />
</p>

</div>

I am an undergraduate student majoring in **Network Engineering** at [Henan University](https://www.henu.edu.cn/) (Double First-Class), graduating in 2027. I am looking for opportunities in **AI Agent development**, with a focus on long-horizon task orchestration, tool use, async performance optimization, and reliable execution.

I enjoy turning complex model capabilities into production-grade engineering systems — building agents that can plan, execute, recover, and deliver real business value. My long-term vision is **embodied intelligence**: giving Agents real hands in the physical world, so they can move from reasoning on screens to perceiving and acting in reality.

## 🧠 Professional Skills

- **Agent frameworks:** LangGraph (SubGraph orchestration, PostgreSQL Checkpointer state persistence, interrupt human-in-the-loop checkpoints), LangChain, Plan-and-Execute paradigm, and multi-stage workflow design for long-horizon task reliability (checkpoint resume, node-level replay). Familiar with MCP protocol and tool dispatch.
- **LLM application engineering:** Prompt Engineering (system prompt design, Few-Shot), SSE streaming interface development, Function Calling, structured output (JSON Mode / with_structured_output layered approach), and multi-model dynamic routing with cost optimization — shipped practice that reduced inference cost by 40%.
- **Async & high availability:** Deep understanding of Python async IO (asyncio.gather concurrent scheduling, run_in_executor for sync API coroutinization), exponential backoff retry, circuit breaker three-state model, rate limiting, and server-side fault recovery with exception handling matrices.
- **Agent observability:** LangSmith full-link tracing, structlog structured logging, request_id correlation across multi-coroutine contexts, node-level performance monitoring, token cost metering, and LLM call instrumentation.
- **Backend & testing:** FastAPI for RESTful APIs and SSE streaming endpoints, pytest unit/integration testing with 70%+ core module coverage, Git, Docker, and Linux development environments.
- **Databases & storage:** PostgreSQL (state persistence design, Checkpointer four-table schema, indexing principles, transaction isolation levels), MySQL, Redis.

## 💼 Internship Experience

### 🔵 ByteDance · Ocean Engine Qianchuan Creative Tools · Agent Development Intern

`2026.03 - 2026.07`

Built agent-powered creative analysis pipelines for advertisers' livestream material production, optimizing video processing architecture and LLM inference performance at scale.

- **Browser-side video processing architecture refactor:** Reconstructed the end-to-end pipeline as a pure-frontend FFmpeg.wasm architecture to solve large-file transcoding bottlenecks. Used WORKERFS virtual filesystem for zero-copy video mounting, enabling GB-level on-demand file reading in the browser. Reduced memory usage from 5GB to **50MB**; transcoded video to 16kHz mono MP3 before upload, shrinking upload volume from 2.5GB to 30MB (**99% reduction**), completely removing server-side FFmpeg dependency and enabling horizontal Worker scaling.
- **AI clip analysis pipeline performance optimization:** Replaced serial LLM batch calls with async concurrent execution (Semaphore rate limiting for API quotas). Split fixed system prompts from dynamic transcription content to trigger KV prefix cache, reducing token cost to **1/10**. Used JSON Mode for forced structured output, eliminating format parsing failures and invalid retries. Reduced single-task latency from 60s to **12s**, with inference cost down **60%**.
- **High-concurrency task scheduling & fault tolerance:** Designed a Redis List-based async task queue with atomic enqueue on the API side and blocking dequeue on the Worker side, paired with distributed locks to prevent duplicate consumption. Implemented a "terminal-state persistence" model — results written in a single transaction only after both ASR and LLM analysis succeed; failures trigger rollback and re-enqueue. Added zombie-task scanning with retry limits (3 attempts then manual alert), covering Worker crashes and long-task interruptions to guarantee **no task loss, no duplicate execution**.

### 🟣 MiniMax (Xiyi Technology) · Product R&D · Agent Backend Development Intern

`2025.11 - 2026.02`

Built long-horizon multi-agent workflow systems focused on reliability, performance, and cost efficiency.

- **Long-horizon multi-agent workflow orchestration:** Addressed single-agent planning drift, non-resumable interruptions, and unchecked outputs with a LangGraph-based three-stage state machine: task decomposition → parallel execution → result validation. Used SubGraphs to decouple each stage as independent orchestration units. Integrated PostgreSQL Checkpointer for runtime state persistence and interrupt human-review checkpoints, supporting checkpoint resume, history rollback, and node-level incremental retry — narrowing fault recovery granularity from full-graph restart to **single-node replay**.
- **Multi-subtask parallel execution optimization:** Solved high-latency serial tool calls and synchronous API event-loop blocking with asyncio.gather concurrent scheduling. Used run_in_executor to coroutinize synchronous tool calls, reducing total multi-tool execution time by **70%**. Added exponential backoff retry (1s→2s→4s+jitter, covering only 429/5xx/timeouts) to handle tool service flakiness without overwhelming downstream.
- **Inference cost optimization & structured output:** Built a dynamic model routing system by task complexity — lightweight tool calls and dialogue routed to M2.5-highspeed, deep reasoning and long-horizon tasks to M2.5 flagship. Used with_structured_output + Pydantic Schema to constrain Tool Call parameters; for precision metering nodes, used JSON Mode + manual parsing with token accounting. Reduced inference cost by **40%** without quality degradation.

## 🛠️ Project Experience

### [EndlessCode](https://github.com/Dream-will-come-true-oneday/EndlessCode) · Independent Development

**Lightweight terminal Coding Agent** · `Python` · `MCP`

EndlessCode is a terminal-based coding Agent that supports multiple LLM providers and MCP extensions. It is designed around a complete loop of reasoning, tool calling, result handling, and continued action.

- **Architecture:** independently built the terminal UI, Agent execution engine, tool sandbox, and memory management modules with a modular design.
- **Multi-LLM adaptation:** unified different providers' streaming protocols behind an event-driven interface, enabling zero-configuration model switching.
- **MCP dynamic dispatch:** created a local tool discovery index with search-triggered Schema injection, reducing context usage by 82% in tool libraries with hundreds of definitions.
- **Context compression:** designed two-level history compression and Function Calling pair validation to support hours-long coding sessions without losing critical context.
- **Security controls:** implemented a five-layer defense chain covering sandbox isolation, path filtering, permission checks, and human-in-the-loop approval, with explainable audit records.
- **Memory evolution:** built an asynchronous memory extraction engine that records user preferences and corrections across sessions, reducing repeated instruction overhead.

## 🎓 Education

**Henan University** · Network Engineering · Undergraduate

`2023.09 - 2027.06`

## 🔭 Long-term Vision

I want to help build the bridge from **digital intelligence to physical action**. The goal is not only to make Agents better at answering questions, but to give them the perception, tools, and eventually the physical hands needed to understand and act in the real world.

<div align="center">

[GitHub](https://github.com/Dream-will-come-true-oneday) · [EndlessCode](https://github.com/Dream-will-come-true-oneday/EndlessCode) · [Email](mailto:13609048665@163.com)

<sub>Building useful agents, one tool call at a time.</sub>

</div>
