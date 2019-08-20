---
title: "No compromises: distributed transactions with consistency, availability, and performance"
authors: "Aleksandar Dragojevic, Dushyanth Narayanan, Ed Nightingale, Matthew Renzelmann, <b>Alex Shamis</b>, Anirudh Badam, Miguel Castro"
collection: publications
permalink: /publication/no-compromises-distributed-transactions-with-consistency
excerpt: 'In this paper, we show that there is no need to compromise in modern data centers. We show that a main memory distributed computing platform called FaRM can provide distributed transactions with strict serializability, high performance, durability, and high availability.'
date: 2015-10-05
paperurl: 'http://ashamis.github.io/files/no-compromises-distributed-transactions-with-consistency.pdf'
venue: 'Symposium on Operating Systems Principles (SOSP)'
---
Transactions with strong consistency and high availability simplify building and reasoning about distributed systems. However, previous implementations performed poorly. This forced system designers to avoid transactions completely, to weaken consistency guarantees, or to provide single-machine transactions that require programmers to partition their data. In this paper, we show that there is no need to compromise in modern data centers. We show that a main memory distributed computing platform called FaRM can provide distributed transactions with strict serializability, high performance, durability, and high availability. FaRM achieves a peak throughput of 140 million TATP transactions per second on 90 machines with a 4.9 TB database, and it recovers from a failure in less than 50 ms. Key to achieving these results was the design of new transaction, replication, and recovery protocols from first principles to leverage commodity networks with RDMA and a new, inexpensive approach to providing non-volatile DRAM.

<small>
Permission to make digital or hard copies of part or all of this work for personal or classroom use is granted without fee provided that copies are not made or distributed for profit or commercial advantage and that copies bear this notice and the full citation onthe first page. Copyrights for third-party components of this work must be honored. For all other uses, contact the owner/author(s).
</small>

[Download paper here](/files/no-compromises-distributed-transactions-with-consistency.pdf)

[Download BibTex here](/files/no-compromises-distributed-transactions-with-consistency.bib)

<iframe width="560" height="315" scrolling="no" src="//av.tib.eu/player/42950" frameborder="0" allowfullscreen></iframe>
