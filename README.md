<div align="center">

# Leonardo · 杨涛华

### AI Agent Developer · Python / Java · Agent Infrastructure

<p>
  <a href="https://github.com/Dream-will-come-true-oneday"><img src="https://img.shields.io/badge/GitHub-Dream--will--come--true--oneday-181717?style=flat-square&logo=github" alt="GitHub profile" /></a>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/MCP-111827?style=flat-square" alt="MCP" />
</p>

</div>

I am an undergraduate student majoring in **Network Engineering** at [Henan University](https://www.henu.edu.cn/), graduating in 2027. I am looking for opportunities in **AI Agent development**, with a focus on agent workflows, tool use, retrieval, long-context reasoning, and reliable execution.

I enjoy turning complex model capabilities into usable engineering systems. My long-term vision is **embodied intelligence**: giving Agents real hands in the physical world, so they can move from reasoning on screens to perceiving and acting in reality.

## 🧠 Professional Skills

- **Agent frameworks:** LangChain, LangGraph, ReAct, Plan-and-Solve, and multi-agent collaboration architecture.
- **LLM application engineering:** Prompt Engineering, Few-Shot prompting, output constraints, SSE streaming, long-context optimization, and Claude Code-assisted development.
- **RAG systems:** document chunking, Embedding, vector storage and retrieval, recall tuning, knowledge-base incremental updates, and long-document question answering.
- **Backend engineering:** Python, FastAPI, RESTful API design, asynchronous IO, multithreading, decorators, Git, and Docker.
- **Storage and databases:** MySQL, Redis, database design, query optimization, indexing principles, and transaction isolation.
- **Computer science foundations:** data structures and algorithms, complexity analysis, TCP/IP, HTTP/HTTPS, SSE, WebSocket, process/thread models, and IO models.

## 💼 Internship Experience

### 🔵 BlueFocus · AI Agent Development Intern

`2026.03 - 2026.07`

Built AI Agent tools for marketing research, helping marketing, strategy, and operations teams collect and organize industry, brand, and competitor intelligence more efficiently.

- **Multi-agent architecture:** helped decompose research into 8 specialist nodes and built a LangGraph state machine with rule-based and LLM-based intent routing. Reduced system hallucination from 25% to below 8% and improved factual citation accuracy from 76% to 94%.
- **Long-context processing:** developed a two-stage dynamic filtering engine with on-demand source reading and extractive paragraph localization for documents over 4k tokens. Reduced invalid token consumption by 80% and shortened report drafting from several hours to under 30 minutes.
- **Iterative research loop:** introduced an Analyst + Reflect correction cycle that evaluates information coverage and triggers targeted follow-up searches. Increased sub-question coverage from 65% to 88% while keeping supplementary searches within 1-2 rounds.
- **Vector database governance:** implemented scheduled polling, last-updated pre-filtering, hash-based change detection, and atomic delete-then-insert updates to keep marketing knowledge bases synchronized with source data.

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

## 🌐 Open Source Experience

### [Open Connector](https://github.com/oomol-lab/open-connector) · Contributor

**Merged:** [feat(bluesky): add authenticated timeline action · PR #392](https://github.com/oomol-lab/open-connector/pull/392) · `2026.08.21`

Open Connector is an open-source connector gateway that makes SaaS capabilities reusable by AI Agents through SDK, CLI, MCP, HTTP, and OpenAPI interfaces.

This contribution came from the secondary development of [BestBlogs](https://github.com/Dream-will-come-true-oneday/BestBlogs). The goal was to let an Agent continuously read the latest posts from a logged-in user's followed accounts without coupling authentication, pagination, and response mapping to one business application.

- Added the Bluesky `get_timeline` Action for authenticated home-timeline access.
- Aligned input and output Schemas with the official Bluesky lexicon, including `algorithm`, `limit`, `cursor`, and feed item structures.
- Added runtime handling, validation, and test coverage so other Agent projects can reuse the capability through MCP or HTTP configuration.

## 🎓 Education

**Henan University** · Network Engineering · Undergraduate

`2023.09 - 2027.06`

## 🔭 Long-term Vision

I want to help build the bridge from **digital intelligence to physical action**. The goal is not only to make Agents better at answering questions, but to give them the perception, tools, and eventually the physical hands needed to understand and act in the real world.

<div align="center">

[GitHub](https://github.com/Dream-will-come-true-oneday) · [EndlessCode](https://github.com/Dream-will-come-true-oneday/EndlessCode) · [Open Connector PR #392](https://github.com/oomol-lab/open-connector/pull/392) · [Email](mailto:13609048665@163.com)

<sub>Building useful agents, one tool call at a time.</sub>

</div>
