---
title: "Fast General Distributed Transactions with Opacity"
collection: publications
permalink: /publication/fast-general-distributed-transactions-with-opacity
excerpt: 'This paper extends the design of FaRM — which provides strict serializability only for committed transactions — to provide opacity while maintaining FaRM’s high throughput, low latency, and high availability within a modern data center. It uses timestamp ordering based on real time with clocks synchronized to within tens of microseconds across a cluster, and a failover protocol to ensure correctness across clock master failures.'
date: 2019-06-30
paperurl: '/files/fast-general-distributed-transactions-with-opacity.pdf'
venue: 'ACM SIGMOD International Conference on Management of Data'
---
Transactions can simplify distributed applications by hiding data distribution, concurrency, and failures from the application developer. Ideally the developer would see the abstraction of a single large machine that runs transactions sequentially and never fails. This requires the transactional subsystem to provide opacity (strict serializability for both committed and aborted transactions), as well as transparent fault tolerance with high availability. As even the best abstractions are unlikely to be used if they perform poorly, the system must also provide high performance.

Existing distributed transactional designs either weaken this abstraction or are not designed for the best performance within a data center. This paper extends the design of FaRM — which provides strict serializability only for committed transactions — to provide opacity while maintaining FaRM’s high throughput, low latency, and high availability within a modern data center. It uses timestamp ordering based on real time with clocks synchronized to within tens of microseconds across a cluster, and a failover protocol to ensure correctness across clock master failures. FaRM with opacity can commit 5.4 million neworder transactions per second when running the TPC-C transaction mix on 90 machines with 3-way replication.

[Download paper here](/files/fast-general-distributed-transactions-with-opacity.pdf)

[Download BibTex here](/files/fast-general-distributed-transactions-with-opacity.bib)