---
title: "Auditable and Performant Byzantine Consensus for Permissioned Ledgers"
authors: "Alex Shamis"
collection: publications
permalink: /publication/Auditable-and-Performant-Byzantine-Consensus-for-Permissioned-Ledgers
excerpt: 'This thesis explores how permissioned ledgers and their consensus protocols can be made auditable in perpetuity; even when all replicas collude and re-write the ledger. It also addresses how Byzantine consensus protocols can be changed to increase the execution throughput of complex transactions.'
date: 2023-05-01
paperurl: '/files/Auditable-and-Performant-Byzantine-Consensus-for-Permissioned-Ledgers.pdf'
venue: 'Imperial College London, Department of Computing'
---

This thesis explores how permissioned ledgers and their consensus protocols can be made auditable in perpetuity; even when all replicas collude and re-write the ledger. It also addresses how Byzantine consensus protocols can be changed to increase the execution throughput of complex transactions. This thesis makes the following contributions:

1. **Always auditable Byzantine consensus protocols**. We present a permissioned ledger system that can assign blame to individual replicas regardless of how many of them misbehave. This is achieved by signing and storing consensus protocol messages in the ledger and providing clients with signed, universally-verifiable receipts.
2. **Performant transaction execution with hardware accelerators**. Next, we describe a cloud-based ML inference service that provides strong integrity guarantees, while staying compatible with current inference APIs. We change the Byzantine consensus protocol to execute machine learning (ML) inference computation on GPUs to optimize throughput and latency of ML inference computation.
3. **Parallel transactions execution on multi-core CPUs**. Finally, we introduce a permissioned ledger that executes transactions, in parallel, on multi-core CPUs. We separate the execution of transactions between the primary and secondary replicas. The primary replica executes transactions on multiple CPU cores and creates a dependency graph of the transactions that the backup replicas utilize to execute transactions in parallel.

[Download thesis here](/files/Auditable-and-Performant-Byzantine-Consensus-for-Permissioned-Ledgers.pdf)

[Download BibTex here](/files/Auditable-and-Performant-Byzantine-Consensus-for-Permissioned-Ledgers.bib)
