<div align="center">

# Abhishek M R

### Software Engineer • Systems, Quant & Full-Stack Architectures

Building ultra-low latency matching engines, distributed backend architectures, stream backpressure proxies, and full-stack engineering platforms.

**Bangalore, India** • Open to High-Impact Engineering & Innovation Teams

[![Portfolio](https://img.shields.io/badge/Live_Portfolio-050914?style=for-the-badge&logo=vercel&logoColor=4D7CFF)](https://portfolio-abhi-byte62.vercel.app/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abhi-byte62)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhishekmr029/)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://leetcode.com/u/playboldAbhi)
[![Codeforces](https://img.shields.io/badge/Codeforces-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white)](https://codeforces.com/profile/playboldAbhi)
[![Email](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mrabhisheak@gmail.com)

</div>

---

## 🧭 Engineering Focus

| Area | Production Focus & Systems Built |
|:---|:---|
| **Low-Latency & Quant Systems** | C++17 fixed-point LOB matching engines, FIFO queue positioning, Hawkes process intensity modeling, sub-microsecond latency benchmarks (`~220ns`). |
| **Distributed Systems & Backend** | Spring Boot 3 microservices, Node.js event runtimes, RabbitMQ asynchronous queues, Redis rate-limiting & caching, WebSocket synchronization. |
| **System Security & Networking** | SSRF & DNS-rebinding perimeter guards, dynamic SNI certificate synthesis, TCP/TLS stream backpressure, PCAP binary parsers. |
| **Full-Stack & Reactive State** | React 19 / 18, TypeScript, optimistic concurrency control (OCC), TanStack Query optimistic mutations, Three.js WebGL GPU instancing. |
| **Databases & Persistence** | PostgreSQL 16/17 (DDL partitioning, GIN indexes, atomic transactions), Prisma ORM, Redis 7.2 (Pub/Sub, TTL invalidation). |
| **Infrastructure & Reliability** | Docker & multi-container Compose, CI/CD pipelines, Vitest unit test suites, hardware profiling with GCC `-O3`. |

---

## 🛠️ Technical Stack

Languages │ C++17 • Java 21 • Python 3.10 • JavaScript / TypeScript (ESNext) • C • SQL Backend & APIs │ Spring Boot 3 • Node.js & Express • FastAPI • RabbitMQ • Socket.io • REST & GraphQL Frontend & UI │ React 19 / 18 • TypeScript • Tailwind CSS • Three.js / WebGL • Vite • TanStack Query Data & Caching │ PostgreSQL 17/16 • Redis 7.2 • Prisma ORM • MongoDB • Fixed-Point int64 Math Networking/Sec │ TLS Termination • Ephemeral SNI • SSRF Shield • DNS Rebinding • PCAP Parsers Tools & Infra │ Docker & Docker Compose • Git & GitHub Actions • Linux / POSIX Shell • GCC -O3


---

## 🚀 Featured Engineering Case Studies

### 1. [StackLens — Website Engineering Intelligence & DAG Inference Engine](https://github.com/abhi-byte62/stackl)
> Developer-focused intelligence platform performing safe deep reverse-engineering of public web systems to infer full backend microservice topologies, database schemas, and caching tiers.

**Tech:** Java 21 • Spring Boot 3 • React 19 • TypeScript • RabbitMQ • PostgreSQL 16 • Redis 7.2 • Tailwind CSS • Docker
- **200+ Weighted Signature Rules:** Evaluates technologies across 16 categories with concrete evidence trails (headers, DOM, scripts, TLS).
- **SSRF & DNS-Rebinding Shield:** Enforces strict RFC 1918 private subnet blacklisting (`10.0.0.0/8`, `127.0.0.1`, `169.254.169.254`) and IP pinning before socket dispatch.
- **Interactive System Architecture DAG:** Generates visual component flows distinguishing directly *Observed* layers from *Inferred* microservices.
- **Engineering Blueprint Generator:** Auto-synthesizes production PostgreSQL DDL schemas, REST/GraphQL API contracts, RS256 JWT auth flows, and a 4-phase rollout plan.

---

### 2. [LiquidityLens — Event-Driven LOB & C++ Execution Simulator](https://github.com/abhi-byte62/liqudity)
> Quantitative research platform and deterministic matching core for studying limit order book dynamics, FIFO fill probabilities, and latency sensitivity.

**Tech:** C++17 (GCC -O3) • Python 3.10 • FastAPI • React 19 • Fixed-Point Math • Hawkes Processes • WebSocket • Docker
- **High-Throughput Core:** Achieves **4.5M+ events/sec** and **~220ns average event latency** using single-threaded fixed-point `int64_t` arithmetic (+110% over floating-point).
- **FIFO Queue Decay Dynamics:** Analyzes fill decay across 7 queue-ahead tiers over 17,500 controlled Monte Carlo trials (Seed 42) with 95% Wilson binomial confidence bounds.
- **Adverse Selection Markouts:** Multi-horizon post-fill trajectories across 7 discrete windows (1ms → 1s) under strict cash-invariant P&L.
- **Microsecond Latency Budget:** Quantifies fill degradation across 10µs, 50µs, 100µs, 250µs, and 500µs simulated execution delays.

---

### 3. [TaskFlow — Real-Time Collaborative Kanban & Distributed State Engine](https://github.com/abhi-byte62/taskflow)
> Real-time collaborative workspace built to eliminate write-conflicts through optimistic concurrency control and float-based drag positioning.

**Tech:** React 18 • Node.js • Express • PostgreSQL 17 • Prisma ORM • Socket.io • TanStack Query • @dnd-kit • Tailwind CSS
- **Optimistic Concurrency Control (OCC):** Version-checked mutating transactions prevent dirty writes and race conditions during simultaneous board edits.
- **O(1) Drag Reordering:** Uses midpoint float positioning with automatic O(n) column rebalancing when gap density drops below `0.001 delta`.
- **Sub-10ms Peer Synchronization:** Bi-directional Socket.io event bus with live room-level presence and instant cache rollback on network failure.
- **Hierarchical RBAC & Audit Trails:** Server-enforced permissions and atomic audit logging across multi-tenant workspaces.

---

### 4. [Packet Sniffer 3D — Real-Time PCAP & WebGL Spatial Topology](https://github.com/abhi-byte62/packet-sniffer-3d-)
> Interactive network protocol visualizer translating raw binary PCAP frame captures into a GPU-instanced 3D topology.

**Tech:** Three.js • WebGL • JavaScript • Binary PCAP Parser • Zero-Copy ArrayBuffers • Vite
- **50K Packets @ 60 FPS:** Streams 50,000+ simultaneous packet trajectories rendered via WebGL instancing in only **3 GPU draw calls**.
- **Zero-Copy Ingestion:** Low-level `ArrayBuffer` slice parser extracting link-layer, IP, and TCP/UDP headers directly from binary streams.
- **Security & Inspection:** Real-time hex payload viewer, protocol filtering, and TLS-aware sensitive payload masking.

---

### 5. [Specter Proxy — Stream Backpressure & Ephemeral TLS Interception Proxy](https://github.com/abhi-byte62/specter-proxy)
> Stream-oriented forward proxy for real-time packet inspection and synthetic network degradation testing.

**Tech:** Node.js Streams • TLS Interception (MITM) • Dynamic SNI • Backpressure Flow Control
- **Strict Stream Backpressure:** Maintains a steady **~35MB heap footprint** under heavy multi-gigabit throughput by synchronizing high-watermark drain events.
- **Dynamic SNI Synthesis:** Ephemeral in-memory TLS certificate generator signed against a local CA on the fly.
- **Network Degradation:** Configurable jitter injection, packet drop emulation, and response tampering with `<4.2ms` latency overhead.

---

## 📈 System Architecture & Research Philosophy

┌──────────────────────────────────────────────────────────────────┐
│ "Build it. Measure it. Profile it. Optimize it." │ │ │ │ 1. Invariant Correctness → Math-verified state & zero leaks │ │ 2. Mechanical Sympathy → Cache locality, fixed-point math │ │ 3. Defensive Perimeter → Pre-connection SSRF & DNS pinning │ │ 4. Deterministic Testing → Seeded trials, OCC conflict tests │ 
└──────────────────────────────────────────────────────────────────┘


---

<div align="center">

### 🤝 Let's Connect & Build

Open to Software Engineering roles (Systems, Backend, Distributed Infrastructure, Quant Dev) and innovative product teams.

📫 **Email:** [mrabhisheak@gmail.com](mailto:mrabhisheak@gmail.com) • 🌐 **Portfolio:** [View Case Studies](https://portfolio-abhi-byte62.vercel.app/) • 💼 **LinkedIn:** [/in/abhishekmr029](https://www.linkedin.com/in/abhishekmr029/)

</div>
