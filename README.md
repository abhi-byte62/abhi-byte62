# Abhishek M R

Hey! I'm Abhishek ([@abhi-byte62](https://github.com/abhi-byte62)), a Computer Science undergrad based in Bangalore, India (graduating 2027).

I spend most of my time working on **low-latency systems**, **distributed backends**, and **security tooling** in C++, Java, and TypeScript. I care a lot about deterministic execution, zero-copy I/O, concurrency primitives, and measuring things instead of guessing.

[Portfolio](https://abhishekmr.vercel.app/) | [LinkedIn](https://www.linkedin.com/in/abhishekmr029/) | [LeetCode](https://leetcode.com/u/playboldAbhi/) | [Codeforces](https://codeforces.com/profile/playboldAbhi) | [Email](mailto:mrabhisheak@gmail.com)

---

## Upstream Open Source Contributions

I contribute to core infrastructure, database engines, and protocol runtimes:

- **[valkey-io/valkey](https://github.com/valkey-io/valkey)** *(C)*: Fixed integer overflow handling during stream trimming (`src/t_stream.c`), removed non-reentrant static compression buffers in RDB serialization (`src/rdb.c`), and modularized key eviction internals (`src/evict.c`).
- **[fastify](https://github.com/fastify)** *(TypeScript / JS)*: Added `$ref` schema resolution to TypeBox validator compiler, enabled OpenAPI 3.x path parameter serialization in `fastify-swagger`, and fixed compiler type signatures in `ajv-compiler`.
- **[QuantConnect/Lean](https://github.com/QuantConnect/Lean)** & **[quickfix](https://github.com/quickfix/quickfix)** *(C#, C++)*: Fixed non-USD futures settlement cash adjustments and lunch-break market bar calculations in Lean; resolved socket disconnect callback firing on session terminations in QuickFIX.
- **[unjs](https://github.com/unjs)** *(TypeScript)*: Propagated `AbortSignal` through `proxyFetch` in `httpxy` to close orphaned upstream sockets, and fixed line-terminator regex edge cases in `pathe`.

---

## Projects

### [TradeForge](https://github.com/abhi-byte62/tradeforge)
*Real-time paper trading platform & market simulator* | [Interactive Overview](https://abhishekmr.vercel.app/tradeforge)
- In-memory deterministic FIFO limit order book in TypeScript executing **247k+ orders/sec** (~4.1 us median latency).
- Synchronous pre-trade risk engine with 5x MIS leverage limits, tick increments, and +/-10% circuit bands.
- Geometric Brownian Motion jump-diffusion price simulator streaming Level-2 depth ladders over WebSockets.
- *Tech:* TypeScript, React 19, PostgreSQL, WebSockets, Canvas API, Docker.

### [LiquidityLens](https://github.com/abhi-byte62/liquiditylens)
*Quantitative market microstructure research & LOB matching core* | [Interactive Overview](https://abhishekmr.vercel.app/liquiditylens)
- Deterministic C++17 matching engine processing **4.5M+ events/sec** (~220 ns match latency) using fixed-point `int64_t` arithmetic.
- FIFO queue priority tracking across 7 queue-ahead tiers with synthetic Hawkes process order arrivals.
- Zero look-ahead post-fill markouts to measure adverse selection across 10 us to 500 us simulated latency steps.
- *Tech:* C++17, Python 3.10, FastAPI, React 19, WebSockets, Docker.

### [StackLens](https://github.com/abhi-byte62/stacklens)
*Asynchronous web technology intelligence engine* | [Interactive Overview](https://abhishekmr.vercel.app/stacklens)
- Passive reconnaissance engine evaluating 200+ signatures from HTTP headers, DOM trees, scripts, and TLS characteristics.
- Asynchronous scanning pipeline powered by Spring Boot and RabbitMQ to decouple probes from API requests.
- SSRF defense layer validating target IPs against RFC 1918, loopback, and cloud metadata addresses before dispatch.
- *Tech:* Java 21, Spring Boot 3, RabbitMQ, PostgreSQL, Redis, React 19, TypeScript.

### [DontTrust](https://github.com/abhi-byte62/dontTrust)
*Application security assessment platform & AST taint engine* | [Interactive Overview](https://abhishekmr.vercel.app/donttrust)
- AST source-to-sink data flow engine detecting client-side DOM XSS without browser execution overhead.
- Multi-identity differential authorization matrix testing Horizontal BOLA/IDOR and Vertical Privilege Escalation.
- Deterministic SHA-256 state graphs with automated secret redaction and SARIF v2.1.0 report generation.
- *Tech:* TypeScript, Node.js, React 19, Cytoscape.js, Playwright, Vitest, SARIF.

### [Specter Proxy](https://github.com/abhi-byte62/specter-proxy)
*Stream backpressure & TLS inspection proxy* | [Interactive Overview](https://abhishekmr.vercel.app/specter-proxy)
- Forward proxy using Node.js stream flow control (`highWaterMark`) to prevent buffer bloat and cap RAM usage to ~35 MB under heavy load.
- Dynamic TLS interception generating on-the-fly ephemeral certificates for arbitrary SNI hosts via a local CA.
- Chaos engine injecting configurable latency, packet drops, and HTTP faults (502, 408).
- *Tech:* Node.js Streams, TCP, TLS, Dynamic SNI.

### [TaskFlow](https://github.com/abhi-byte62/taskflow)
*Real-time collaborative Kanban with optimistic concurrency* | [Interactive Overview](https://abhishekmr.vercel.app/taskflow)
- Real-time board synchronization with integer revision tags rejecting stale writes via optimistic concurrency control (OCC).
- Fractional midpoint ranking for O(1) drag-and-drop reordering without cascading database updates.
- *Tech:* React, Node.js, PostgreSQL, Prisma, Socket.io, TanStack Query, Tailwind CSS.

### [Packet Sniffer 3D](https://github.com/abhi-byte62/packet-sniffer-3d)
*Binary PCAP parser & WebGL 3D network topology* | [Interactive Overview](https://abhishekmr.vercel.app/packet-sniffer)
- In-browser binary PCAP parser reading raw `ArrayBuffer` views for zero-copy header decoding.
- WebGL instanced rendering displaying 50,000+ simultaneous packet trajectories at 60 FPS in 3 draw calls.
- *Tech:* Three.js, WebGL, JavaScript, Vite, ArrayBuffers.

---

## Tech

- **Languages:** C++17, Java 21, TypeScript, JavaScript, Python, C, SQL
- **Systems & Backend:** Spring Boot 3, Node.js, Express, FastAPI, RabbitMQ, Redis, PostgreSQL, WebSockets
- **Protocols & Security:** TCP, TLS, HTTP/HTTPS, PCAP, Stream Backpressure, AST Analysis, SSRF Defense
- **Frontend & Graphics:** React 19, TypeScript, Tailwind CSS, Three.js, WebGL, Canvas API, TanStack Query
- **Tools & Infra:** Docker, Docker Compose, Linux, Git, GitHub Actions, GCC/Clang, Vitest

---

## Problem Solving

I regularly practice competitive programming and core DSA:
- **LeetCode:** [playboldAbhi](https://leetcode.com/u/playboldAbhi)
- **Codeforces:** [playboldAbhi](https://codeforces.com/profile/playboldAbhi)

---

Feel free to reach out at [mrabhisheak@gmail.com](mailto:mrabhisheak@gmail.com) or connect on [LinkedIn](https://www.linkedin.com/in/abhishekmr029/).