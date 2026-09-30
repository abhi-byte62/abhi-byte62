<div align="center">

# Abhishek M R

### Software Engineer • Systems • Quant • Backend

I build low-latency systems, distributed backends, networking tools, and real-time engineering applications.

**Bangalore, India**

[![Portfolio](https://img.shields.io/badge/Portfolio-050914?style=for-the-badge&logo=vercel&logoColor=4D7CFF)](https://abhishekmr.vercel.app/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abhi-byte62)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhishekmr029/)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/playboldAbhi)
[![Codeforces](https://img.shields.io/badge/Codeforces-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white)](https://codeforces.com/profile/playboldAbhi)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mrabhisheak@gmail.com)

</div>

---

## Engineering Focus

| Area | Focus |
|:---|:---|
| **Systems & Quant** | C++17, fixed-point arithmetic, limit order books, FIFO matching, market simulation, latency benchmarking |
| **Backend & Distributed Systems** | Java, Spring Boot, Node.js, REST, WebSockets, RabbitMQ, Redis, PostgreSQL |
| **Networking & Security** | TCP/TLS, HTTP proxies, stream backpressure, PCAP parsing, SSRF protection, DNS rebinding protection |
| **Full-Stack Engineering** | React, TypeScript, Vite, Tailwind CSS, TanStack Query, real-time state synchronization |
| **Databases & Persistence** | PostgreSQL, Prisma, Redis, transactions, indexing, optimistic concurrency |
| **Infrastructure** | Docker, Docker Compose, GitHub Actions, Linux/POSIX shell, GCC optimization |

---

# Featured Projects

## 1. TradeForge — Real-Time Paper Trading & Market Simulation Platform

[![Repository](https://img.shields.io/badge/GitHub-TradeForge-181717?style=flat&logo=github)](https://github.com/abhi-byte62/tradeforge)

A web-based paper trading terminal built around a deterministic price-time-priority matching engine, pre-trade risk validation, market simulation, and real-time WebSocket streaming.

**Tech:** TypeScript • React • Node.js • PostgreSQL • Redis • RabbitMQ • WebSockets • Docker

### Engineering Highlights

- **Deterministic Matching Engine:** Double-sided L2/L3 order books with price-time priority, FIFO execution, partial fills, multi-level fills, cancellations, and order modifications.

- **Multiple Order Types:** Supports `MARKET`, `LIMIT`, `STOP_LOSS`, and `STOP_LOSS_LIMIT` order lifecycles.

- **Pre-Trade Risk Engine:** Validates margin, holdings, quantity, tick size, circuit limits, and product-specific trading constraints before execution.

- **Idempotent Order Submission:** Uses idempotency keys to prevent duplicate HTTP submissions from producing duplicate executions.

- **Market Simulation:** Combines Geometric Brownian Motion, Ornstein-Uhlenbeck mean reversion, and jump diffusion with deterministic seeded simulation.

- **Real-Time Market Data:** Generates L2 depth and multi-timeframe OHLC data and distributes updates through selective WebSocket symbol subscriptions.

- **Portfolio Engine:** Tracks positions, weighted average cost, realized P&L, unrealized P&L, available margin, and square-off operations.

- **Performance:** Matching engine benchmarked at **232,633 orders/sec** with **4.20 µs p50**, **8.10 µs p95**, and **10.40 µs p99** matching latency under the documented benchmark workload.

- **Testing:** **21/21 unit and integration tests passing**, covering matching, risk validation, deterministic simulation, P&L, and idempotency.

> Benchmark figures measure the in-memory matching engine and should not be interpreted as end-to-end network or browser latency.

---

## 2. LiquidityLens — Event-Driven LOB & C++ Execution Simulator

[![Repository](https://img.shields.io/badge/GitHub-LiquidityLens-181717?style=flat&logo=github)](https://github.com/abhi-byte62/liqudity)

A quantitative research platform for studying limit order book dynamics, FIFO queue position, fill probability, adverse selection, and execution latency.

**Tech:** C++17 • GCC `-O3` • Python • FastAPI • React • Fixed-Point Arithmetic • Hawkes Processes • WebSocket • Docker

### Engineering Highlights

- **High-Throughput Matching Core:** C++17 matching engine using fixed-point `int64_t` arithmetic, benchmarked at **4.5M+ events/sec** with approximately **220 ns average event latency** under the documented workload.

- **FIFO Queue Analysis:** Models fill probability across **7 queue-ahead tiers** using controlled Monte Carlo simulations with deterministic seeds.

- **Execution Analysis:** Measures post-fill price movement across multiple time horizons to study adverse selection and execution quality.

- **Latency Sensitivity:** Simulates execution delays from **10 µs to 500 µs** and measures their effect on simulated fills.

- **Deterministic Experiments:** Seeded simulations allow experiments to be reproduced and compared across different execution configurations.

---

## 3. StackLens — Website Engineering Intelligence Platform

[![Repository](https://img.shields.io/badge/GitHub-StackLens-181717?style=flat&logo=github)](https://github.com/abhi-byte62/stackl)

A developer-focused platform that analyzes public web applications and infers their underlying technology stack from HTTP, HTML, JavaScript, TLS, and network fingerprints.

**Tech:** Java 21 • Spring Boot 3 • React • TypeScript • RabbitMQ • PostgreSQL • Redis • Tailwind CSS • Docker

### Engineering Highlights

- **Technology Detection Engine:** Uses **200+ weighted signatures** across multiple technology categories with evidence collected from HTTP headers, DOM structures, scripts, TLS characteristics, and other observable signals.

- **Asynchronous Scanning Pipeline:** Uses Spring Boot and RabbitMQ to process website scans asynchronously rather than blocking the API request.

- **SSRF Protection:** Implements private-network and metadata-address filtering together with DNS/IP validation before outbound connections.

- **Technology Confidence:** Produces evidence-backed classifications instead of treating every detected technology as equally certain.

- **Architecture Visualization:** Converts detected relationships into an interactive architecture graph separating directly observed components from inferred components.

- **Caching & Persistence:** Uses Redis for cache-oriented workloads and PostgreSQL for persistent scan and analysis data.

---

## 4. Specter Proxy — Stream Backpressure & TLS Interception Proxy

[![Repository](https://img.shields.io/badge/GitHub-Specter_Proxy-181717?style=flat&logo=github)](https://github.com/abhi-byte62/specter-proxy)

A stream-oriented HTTP/TLS proxy designed for traffic inspection and controlled network degradation experiments.

**Tech:** Node.js • Streams • TCP • TLS • Dynamic SNI • Backpressure Control

### Engineering Highlights

- **Stream Backpressure:** Uses Node.js stream flow control and high-watermark handling to prevent uncontrolled buffering under sustained traffic.

- **Dynamic TLS Interception:** Generates ephemeral certificates for requested SNI hosts using a locally trusted CA.

- **Traffic Simulation:** Supports configurable latency/jitter injection, packet-drop behavior, and response manipulation for network testing.

- **Memory Stability:** Designed to maintain bounded buffering rather than accumulating entire request/response payloads in memory.

- **Protocol Inspection:** Exposes connection and traffic information while preserving streaming behavior.

---

## 5. TaskFlow — Real-Time Collaborative Workspace

[![Repository](https://img.shields.io/badge/GitHub-TaskFlow-181717?style=flat&logo=github)](https://github.com/abhi-byte62/taskflow)

A real-time collaborative Kanban-style workspace designed around concurrent editing, optimistic updates, and persistent ordering.

**Tech:** React • TypeScript • Node.js • Express • PostgreSQL • Prisma • Socket.io • TanStack Query • dnd-kit • Tailwind CSS

### Engineering Highlights

- **Optimistic Concurrency Control:** Uses version-checked transactions to prevent conflicting concurrent updates from silently overwriting each other.

- **Real-Time Synchronization:** Socket.io distributes board changes and presence information between connected clients.

- **Optimistic UI:** TanStack Query mutations update the interface immediately and roll back when the server rejects an operation.

- **Efficient Ordering:** Uses midpoint-based positioning for drag-and-drop operations and rebalances a column when ordering gaps become too small.

- **Multi-Tenant Authorization:** Server-side permission checks isolate workspace and board operations between users.

- **Audit Trail:** Records important workspace mutations for traceability.

---

## 6. Packet Sniffer 3D — PCAP & WebGL Network Visualizer

[![Repository](https://img.shields.io/badge/GitHub-Packet_Sniffer_3D-181717?style=flat&logo=github)](https://github.com/abhi-byte62/packet-sniffer-3d-)

A browser-based network visualization tool that parses binary PCAP captures and renders packet flows as an interactive 3D topology.

**Tech:** Three.js • WebGL • JavaScript • Vite • Binary PCAP Parsing • ArrayBuffers

### Engineering Highlights

- **Binary PCAP Parser:** Parses packet capture data directly from binary buffers and extracts link-layer, IP, TCP, and UDP information.

- **GPU Rendering:** Uses WebGL instancing to render large numbers of packet trajectories efficiently.

- **Zero-Copy Processing:** Uses `ArrayBuffer` views to minimize unnecessary data copying during packet parsing.

- **Interactive Inspection:** Provides protocol filtering, packet inspection, and hexadecimal payload views.

- **Network Topology:** Converts packet relationships into an interactive 3D representation for exploring traffic flows.

---

# Technical Stack

### Languages

`C++17` `Java 21` `Python` `JavaScript` `TypeScript` `C` `SQL`

### Backend

`Spring Boot` `Node.js` `Express` `FastAPI` `REST` `WebSockets` `Socket.io`

### Systems & Quant

`Limit Order Books` `FIFO Matching` `Fixed-Point Arithmetic` `Market Simulation` `Hawkes Processes` `Latency Benchmarking`

### Frontend

`React` `TypeScript` `Vite` `Tailwind CSS` `Three.js` `WebGL` `TanStack Query`

### Data & Infrastructure

`PostgreSQL` `Redis` `Prisma` `RabbitMQ` `Docker` `Docker Compose`

### Networking & Security

`TCP` `HTTP` `TLS` `SNI` `Stream Backpressure` `PCAP` `SSRF Protection` `DNS Rebinding Protection`

### Tools

`Git` `GitHub Actions` `Linux` `GCC` `POSIX Shell`

---

# Engineering Approach

I generally optimize around four principles:

### 1. Correctness First

Define invariants and state transitions before optimizing implementation details.

### 2. Measure Before Optimizing

Use reproducible workloads, benchmarks, profiling, and controlled experiments rather than relying on assumptions.

### 3. Keep the Hot Path Simple

Avoid unnecessary allocations, network calls, serialization, and persistence operations inside latency-sensitive paths.

### 4. Design for Failure

Account for retries, duplicate requests, connection loss, concurrent writes, invalid input, and partial failures.

---

# Problem Solving

I regularly practice data structures and algorithms through competitive programming and interview preparation.

**LeetCode:** [playboldAbhi](https://leetcode.com/u/playboldAbhi)

**Codeforces:** [playboldAbhi](https://codeforces.com/profile/playboldAbhi)

---

# Links

**Portfolio:**  
https://abhishekmr.vercel.app/

**GitHub:**  
https://github.com/abhi-byte62

**LinkedIn:**  
https://www.linkedin.com/in/abhishekmr029/

**Email:**  
mrabhisheak@gmail.com

---

<div align="center">

### Build → Measure → Profile → Optimize

Open to Software Engineering, Backend, Systems, Distributed Infrastructure, and Quant Development opportunities.

</div>
