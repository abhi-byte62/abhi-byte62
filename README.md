<div align="center">

# Abhishek M R

### Software Engineer â€¢ Systems â€¢ Quantitative Engineering â€¢ Distributed Backends

Building low-latency matching engines, distributed architectures, network security tooling, and real-time state synchronization systems.

**Bangalore, India**

[![Portfolio](https://img.shields.io/badge/Portfolio-050914?style=for-the-badge&logo=vercel&logoColor=4D7CFF)](https://abhishekmr.vercel.app/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abhi-byte62)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhishekmr029/)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/playboldAbhi)
[![Codeforces](https://img.shields.io/badge/Codeforces-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white)](https://codeforces.com/profile/playboldAbhi)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mrabhisheak@gmail.com)

</div>

---

## âš¡ Engineering Focus

| Domain | Core Competencies & Technologies |
|:---|:---|
| **Systems & Quant** | C++17, fixed-point integer arithmetic, limit order books, FIFO price-time matching, market simulation, Hawkes processes, latency benchmarking |
| **Backend & Distributed Systems** | Java 21, Spring Boot 3, Node.js, Express, FastAPI, RabbitMQ event queues, Redis caching, PostgreSQL transactions |
| **Security & Networking** | Zero-trust AST data-flow analysis, SSRF protection guards, dynamic TLS interception, stream backpressure flow control, binary PCAP parsing |
| **Real-Time & Full-Stack** | React 19, TypeScript, Vite, WebSockets, Socket.io, TanStack Query, optimistic concurrency control (OCC), Three.js / WebGL |
| **Infrastructure & Tooling** | Docker, Docker Compose, Linux / POSIX shell, GCC `-O3` optimizations, GitHub Actions CI/CD |

---

# ðŸš€ Featured Systems & Projects

## 1. TradeForge â€” Real-Time Paper Trading & Market Simulation Platform

[![Repository](https://img.shields.io/badge/GitHub-TradeForge-181717?style=flat&logo=github)](https://github.com/abhi-byte62/tradeforge)
[![Live Demo](https://img.shields.io/badge/Live_Overview-abhishekmr.vercel.app%2Ftradeforge-blue?style=flat&logo=vercel)](https://abhishekmr.vercel.app/tradeforge)

A modular, high-performance web-based paper trading platform and market simulator featuring an in-memory double-sided order book with deterministic price-time priority matching, synchronous pre-trade risk evaluation, and stochastic tick simulation.

**Tech:** TypeScript â€¢ Node.js â€¢ React 19 â€¢ Native WebSockets â€¢ PostgreSQL â€¢ Tailwind CSS â€¢ Canvas API â€¢ Docker

### Engineering Highlights
- **In-Memory Matching Core:** Deterministic FIFO matching algorithm with $O(1)$ hash-map cancellations, multi-level VWAP fills, and benchmarked execution at **247,000+ orders/sec** (~4.1 Âµs latency).
- **Synchronous Risk Engine:** Enforces pre-trade margin gates (5x MIS leverage), tick size validation, and circuit-breaker bands ($\pm 10\%$) with invariant zero-leakage balance conservation.
- **WebSocket Streaming:** Broadcasts real-time Level-2 depth ladder snapshots and 5-level market feeds to web clients over low-overhead socket connections.
- **Visual Analytics:** Custom Canvas-based interactive candlestick chart and live telemetry dashboard.

---

## 2. LiquidityLens â€” Quantitative Limit Order Book & Microstructure Research

[![Repository](https://img.shields.io/badge/GitHub-LiquidityLens-181717?style=flat&logo=github)](https://github.com/abhi-byte62/liquiditylens)
[![Live Demo](https://img.shields.io/badge/Live_Overview-abhishekmr.vercel.app%2Fliquiditylens-blue?style=flat&logo=vercel)](https://abhishekmr.vercel.app/liquiditylens)

An event-driven market microstructure research platform and C++ simulation engine for studying limit order book dynamics, FIFO queue priority, fill probability, adverse selection, and microsecond-level latency budgets.

**Tech:** C++17 â€¢ GCC `-O3` â€¢ Python 3.10 â€¢ FastAPI â€¢ React 19 â€¢ Fixed-Point Math â€¢ Hawkes Processes â€¢ WebSocket â€¢ Docker

### Engineering Highlights
- **High-Throughput Matching Core:** C++17 matching engine utilizing fixed-point `int64_t` arithmetic (zero floating-point drift), benchmarked at **4.5M+ events/sec** with **~220 ns average event latency**.
- **FIFO Queue Priority Modeling:** Evaluates fill probability decay across **7 queue-ahead tiers** using deterministic Monte Carlo simulations.
- **Adverse Selection Markouts:** Computes multi-horizon post-fill price excursions ($t+10\text{ms}, t+100\text{ms}, t+1\text{s}$) to quantify execution quality without look-ahead bias.
- **Latency Sensitivity Engine:** Simulates execution slip and queue degradation across multi-stage delay envelopes ($10\,\mu\text{s} \to 500\,\mu\text{s}$).

---

## 3. StackLens â€” Website Engineering Intelligence & Reconnaissance Engine

[![Repository](https://img.shields.io/badge/GitHub-StackLens-181717?style=flat&logo=github)](https://github.com/abhi-byte62/stacklens)
[![Live Demo](https://img.shields.io/badge/Live_Overview-abhishekmr.vercel.app%2Fstacklens-blue?style=flat&logo=vercel)](https://abhishekmr.vercel.app/stacklens)

An asynchronous developer intelligence engine that parses and correlates public web application signals to infer infrastructure topologies, protected by SSRF-hardened perimeter guards.

**Tech:** Java 21 â€¢ Spring Boot 3 â€¢ RabbitMQ â€¢ PostgreSQL 16 â€¢ Redis 7.2 â€¢ React 19 â€¢ TypeScript â€¢ Tailwind CSS â€¢ Docker

### Engineering Highlights
- **Signature Detection Engine:** Correlates **200+ weighted signatures** across DOM structures, HTTP response headers, script signatures, and TLS fingerprints.
- **Asynchronous Event-Driven Pipeline:** Leverages RabbitMQ and Spring Boot workers to isolate long-running network probes from API gateways.
- **SSRF Perimeter Shield:** Implements DNS pre-resolution and private subnet filtering (RFC 1918, loopback, link-local, cloud metadata) to block request smuggling and perimeter probing.
- **Architecture DAG Visualization:** Converts detected component relationships into an interactive directed acyclic graph (DAG) distinguishing directly observed vs. inferred dependencies.

---

## 4. DontTrust â€” Application Security & Attack-Surface Intelligence Platform

[![Repository](https://img.shields.io/badge/GitHub-DontTrust-181717?style=flat&logo=github)](https://github.com/abhi-byte62/dontTrust)
[![Live Demo](https://img.shields.io/badge/Live_Overview-abhishekmr.vercel.app%2Fdonttrust-blue?style=flat&logo=vercel)](https://abhishekmr.vercel.app/donttrust)

A distributed web application security assessment platform in TypeScript across 17 monorepo workspaces, integrating discovery, AST source-to-sink data flow analysis, multi-identity differential authorization, and SARIF v2.1.0 reporting.

**Tech:** TypeScript â€¢ Node.js â€¢ React 19 â€¢ Cytoscape.js â€¢ AST Analysis â€¢ WebSockets â€¢ Playwright â€¢ Vitest â€¢ Docker â€¢ SARIF

### Engineering Highlights
- **AST Source-to-Sink Data Flow:** Client-side AST analysis detecting DOM-based XSS pathways and taint propagation with zero third-party runtime dependencies.
- **Differential Authorization Matrix:** Automated multi-identity session analysis testing Horizontal BOLA / IDOR and Vertical Privilege Escalation flaws.
- **Deterministic State Graph:** Generates SHA-256 state graphs with automated secret redaction and industry-standard SARIF v2.1.0 compliance exports.
- **Benchmark Precision:** Achieves 100% precision and zero false positives across reproducible benchmark test suites.

---

## 5. Specter Proxy â€” Stream Backpressure & TLS Interception Proxy

[![Repository](https://img.shields.io/badge/GitHub-Specter_Proxy-181717?style=flat&logo=github)](https://github.com/abhi-byte62/specter-proxy)
[![Live Demo](https://img.shields.io/badge/Live_Overview-abhishekmr.vercel.app%2Fspecter--proxy-blue?style=flat&logo=vercel)](https://abhishekmr.vercel.app/specter-proxy)

A stream-oriented forward proxy designed for live protocol inspection, network fault injection, and controlled network degradation experiments.

**Tech:** Node.js Streams â€¢ TCP â€¢ TLS â€¢ Dynamic SNI â€¢ Backpressure Flow Control

### Engineering Highlights
- **Stream Backpressure Control:** Manages high-watermark pause/resume flow control to prevent buffer bloat and cap heap consumption under sustained multi-gigabit traffic to ~35MB.
- **Dynamic TLS Interception:** Generates on-the-fly ephemeral certificates for arbitrary SNI hostnames signed by a local certificate authority.
- **Chaos Injection Engine:** Programmatic latency throttling, packet drops, and HTTP fault synthesis (502, 408) for resilience testing.

---

## 6. TaskFlow â€” Real-Time Collaborative State Engine

[![Repository](https://img.shields.io/badge/GitHub-TaskFlow-181717?style=flat&logo=github)](https://github.com/abhi-byte62/taskflow)
[![Live Demo](https://img.shields.io/badge/Live_Overview-abhishekmr.vercel.app%2Ftaskflow-blue?style=flat&logo=vercel)](https://abhishekmr.vercel.app/taskflow)

A real-time collaborative Kanban workspace architected around optimistic concurrency control, sub-10ms state synchronization, and conflict-free ordering.

**Tech:** React 18 â€¢ TypeScript â€¢ Node.js â€¢ Express â€¢ PostgreSQL 17 â€¢ Prisma ORM â€¢ Socket.io â€¢ TanStack Query â€¢ @dnd-kit

### Engineering Highlights
- **Optimistic Concurrency Control (OCC):** Integer revision tags reject stale concurrent writes with 409 Conflict triggers, preventing lost updates.
- **Midpoint Float Ranking:** Eliminates cascading $O(N)$ database updates on drag-and-drop operations through fractional index rebalancing.
- **Live State Sync:** Socket.io room-scoped events broadcast board state mutations and cursor presence across connected clients in sub-10ms.

---

## 7. Packet Sniffer 3D â€” Binary PCAP Ingestion & WebGL Spatial Topology

[![Repository](https://img.shields.io/badge/GitHub-Packet_Sniffer_3D-181717?style=flat&logo=github)](https://github.com/abhi-byte62/packet-sniffer-3d)
[![Live Demo](https://img.shields.io/badge/Live_Overview-abhishekmr.vercel.app%2Fpacket--sniffer-blue?style=flat&logo=vercel)](https://abhishekmr.vercel.app/packet-sniffer)

A browser-based network visualization engine that parses binary PCAP captures and renders packet flows as an interactive 3D topology.

**Tech:** Three.js â€¢ WebGL â€¢ JavaScript â€¢ Vite â€¢ Binary PCAP Parsing â€¢ ArrayBuffers

### Engineering Highlights
- **Zero-Copy Binary PCAP Parser:** Extracts Ethernet, IPv4, TCP, and UDP headers directly from raw `ArrayBuffer` views without garbage collection overhead.
- **GPU Instanced Rendering:** WebGL instanced meshes batch 50,000+ simultaneous packet trajectories into 3 draw calls at continuous 60 FPS.

---

# ðŸ“Š GitHub Activity & Metrics

<div align="center">
  <img src="https://github-readme-stats-sigma-five.vercel.app/api?username=abhi-byte62&show_icons=true&theme=tokyonight&hide_border=true&bg_color=050914&title_color=4D7CFF&text_color=94A3B8&icon_color=60A5FA" height="165" alt="GitHub Stats" />
  <img src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=abhi-byte62&layout=compact&theme=tokyonight&hide_border=true&bg_color=050914&title_color=4D7CFF&text_color=94A3B8" height="165" alt="Top Languages" />
</div>

---

# ðŸ›  Comprehensive Technical Stack

### Languages
`C++17` `Java 21` `Python 3.10` `TypeScript` `JavaScript (ESNext)` `C` `SQL`

### Systems, Quant & High-Performance
`Limit Order Books` `Price-Time Matching (FIFO)` `Fixed-Point Arithmetic` `Hawkes Processes` `Latency Sensitivity Modeling` `ArrayBuffer Slicing`

### Backend & Distributed Infrastructure
`Spring Boot 3` `Node.js` `Express` `FastAPI` `RabbitMQ` `PostgreSQL` `Redis` `Prisma ORM` `RESTful APIs` `WebSockets` `Socket.io`

### Security & Networking
`AST Source-to-Sink Flow` `Differential Authorization` `SSRF Perimeter Protection` `DNS Rebinding Guards` `Dynamic TLS Interception` `Stream Backpressure` `Binary PCAP Parsing` `SARIF v2.1.0`

### Frontend & Graphics
`React 19` `TypeScript` `Tailwind CSS` `Three.js` `WebGL` `TanStack Query` `Canvas API` `dnd-kit` `Vite`

### DevOps & Tooling
`Docker` `Docker Compose` `Git` `GitHub Actions` `Linux (POSIX)` `GCC / Clang` `Vitest` `Playwright`

---

# ðŸ“ Core Engineering Principles

1. **Correctness First:** Define invariants, finite state transitions, and arithmetic boundaries before micro-optimizing implementations.
2. **Measure Before Optimizing:** Rely on deterministic benchmarks, profiling, and controlled workloads rather than intuitive assumptions.
3. **Keep the Hot Path Simple:** Eliminate dynamic allocations, heavy serialization, blocking locks, and redundant network hops from latency-critical loops.
4. **Design for Failure:** Plan for asynchronous timeouts, network partitions, concurrent write collisions, and partial degradation across every tier.

---

# ðŸ’¡ Problem Solving & Competitive Programming

- **LeetCode:** [playboldAbhi](https://leetcode.com/u/playboldAbhi)
- **Codeforces:** [playboldAbhi](https://codeforces.com/profile/playboldAbhi)

---

<div align="center">

### Build â†’ Measure â†’ Profile â†’ Optimize

Open to **Software Engineering, Systems, Backend, Distributed Infrastructure, and Quant Development** opportunities.

[![Portfolio](https://img.shields.io/badge/abhishekmr.vercel.app-050914?style=flat-square&logo=vercel)](https://abhishekmr.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhishekmr029/)
[![Email](https://img.shields.io/badge/mrabhisheak@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:mrabhisheak@gmail.com)

</div>