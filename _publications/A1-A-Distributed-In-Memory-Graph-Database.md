---
title: "A1: A Distributed In-Memory Graph Database"
authors: "Chiranjeeb Buragohain, Knut Magne Risvik, Paul Brett, Miguel Castro, Wonhee Cho, Joshua Cowhig, Nikolas Gloy, Karthik Kalyanaraman, Richendra Khanna, John Pao, Matthew Renzelmann, <b>Alex Shamis</b>, Timothy Tan, Shuheng Zheng"
collection: publications
permalink: /publication/A-Framework-for-Building-Confidential-Verifiable-Replicated-Services
excerpt: 'This paper present CCF, a framework to build premissioned confidential blockchains. CCF provides a simple programming model of a highly-available data store and a universally-verifiable log that implements a ledger abstraction. CCF leverages trust in a consortium of governing members and in a network of replicated hardware-protected execution environments to achieve high throughput, low latency, strong integrity and strong confidentiality for application data and code executing on the ledger.'
date: 2020-06-14
paperurl: '/files/A1-A-Distributed-In-Memory-Graph-Database.pdf'
venue: 'ACM SIGMOD International Conference on Management of Data'
---
A1 is an in-memory distributed database used by the Bing search engine to support complex queries over structured data. The key enablers for A1 are availability of cheap DRAM and high speed RDMA (Remote Direct Memory Access) networking in commodity hardware. A1 uses FaRM as its underlying storage layer and builds the graph abstraction and query engine on top. The combination of in-memory storage and RDMA access requires rethinking how data is allocated, organized and queried in a large distributed system. A single A1 cluster can store tens of billions of vertices and edges and support a throughput of 350+ million of vertex reads per second with end to end query latency in single digit milliseconds. In this paper we describe the A1 data model, RDMA optimized data structures and query execution.

[Download paper here](/files/A1-A-Distributed-In-Memory-Graph-Database.pdf)

[Download BibTex here](/files/A1-A-Distributed-In-Memory-Graph-Database.bib)
