# Viet Nguyen

CS @ University of South Florida. I work on backend systems — state, consistency, concurrency, and what happens when things fail mid-write.

**Currently**

- GPU partitioning and scheduling for real-time systems (autonomous driving workloads) at the RTS Lab
- Backend engineering intern at a fintech unicorn — Java, Vert.x, Kafka, Redis, gRPC
- Building internal tooling on C#/.NET and SignalR for the USF Honors College

**Selected work**

[**fault-tolerant-payment-service**](https://github.com/nnviet06/fault-tolerant-payment-service) — Append-only, hash-chained payment ledger on Vert.x. Every debit passes a row lock and a database-enforced invariant, so 100 concurrent withdrawals against one balance produce 0 overdrafts. Idempotency claim, ledger write, and outbox event commit in one ACID transaction: 235 transfers/sec at 0 errors, stranded events recovered in 30 ms median. A 9-scenario JUnit harness boots the real service as a subprocess, kills it mid-transaction, and blacks out Redis to prove each guarantee.

[**honors-inventory-system**](https://github.com/nnviet06/honors-inventory-system) — Rebuilt a single-user prototype into a multi-user system: state moved out of a redeploy-wiped SQLite file into Postgres behind a separately deployed API. Found and fixed a silent multi-tenant bug where every user read the same dataset. Pagination and multi-field filtering pushed out of the browser into indexed queries — 2,000+ items/user, 99% smaller per-request payloads.

**Stack**

<p>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Vert.x-782A90?style=flat-square" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
</p>

Also worked in C, C++, CUDA, TypeScript, React, and Node.

**Reach me** — [LinkedIn](https://www.linkedin.com/in/nnviet/) · [nnviet2016@gmail.com](mailto:nnviet2016@gmail.com)