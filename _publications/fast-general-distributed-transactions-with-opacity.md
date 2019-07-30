---
title: "Fast General Distributed Transactions with Opacity"
authors: "<b>Alex Shamis</b>, Matthew Renzelmann, Stanko Novakovic, Georgios Chatzopoulos, Aleksandar Dragojevic, Dushyanth Narayanan, Miguel Castro"
collection: publications
permalink: /publication/fast-general-distributed-transactions-with-opacity
excerpt: 'This paper extends the design of FaRM — which provides strict serializability only for committed transactions — to provide opacity while maintaining FaRM’s high throughput, low latency, and high availability within a modern data center. It uses timestamp ordering based on real time with clocks synchronized to within tens of microseconds across a cluster, and a failover protocol to ensure correctness across clock master failures.'
date: 2019-06-30
paperurl: '/files/fast-general-distributed-transactions-with-opacity.pdf'
venue: 'ACM SIGMOD International Conference on Management of Data'
---

<strong>Best Paper - Honorable Mention</strong>

Transactions can simplify distributed applications by hiding data distribution, concurrency, and failures from the application developer. Ideally the developer would see the abstraction of a single large machine that runs transactions sequentially and never fails. This requires the transactional subsystem to provide opacity (strict serializability for both committed and aborted transactions), as well as transparent fault tolerance with high availability. As even the best abstractions are unlikely to be used if they perform poorly, the system must also provide high performance.

Existing distributed transactional designs either weaken this abstraction or are not designed for the best performance within a data center. This paper extends the design of FaRM — which provides strict serializability only for committed transactions — to provide opacity while maintaining FaRM’s high throughput, low latency, and high availability within a modern data center. It uses timestamp ordering based on real time with clocks synchronized to within tens of microseconds across a cluster, and a failover protocol to ensure correctness across clock master failures. FaRM with opacity can commit 5.4 million neworder transactions per second when running the TPC-C transaction mix on 90 machines with 3-way replication.

<small>
Permission to make digital or hard copies of all or part of this work for personal or classroom use is granted without fee provided that copies are not made or distributed for profit or commercial advantage and that copies bear this notice and the full citation on the first page. Copyrights for components of this work owned by others than the author(s) must be honored. Abstracting with credit is permitted. To copy otherwise, or republish, to post on servers or to redistribute to lists, requires prior specific permission and/or a fee. Request permissions from permissions@acm.org. SIGMOD ’19, June 30-July 5, 2019, Amsterdam, Netherlands © 2019 Copyright held by the owner/author(s). Publication rights licensed to ACM.
</small>

[Download paper here](/files/fast-general-distributed-transactions-with-opacity.pdf)

[Download BibTex here](/files/fast-general-distributed-transactions-with-opacity.bib)

[Download honorable mention certificate here](/files/fast-general-distributed-transactions-with-opacity-Honorable-mention.pdf)
