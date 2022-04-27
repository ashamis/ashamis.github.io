---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D in Computing, Imperial College London, 2022 (expected)
* B.S. in Computer Science, University of New South Wales, 2009
* B.S. in Mathematics, University of New South Wales, 2009

Work experience
======
* Senior Research Software Engineer, Microsoft Research, 2019 - Current
  * Designed, built, and owned the Byzantine fault tolerance feature for Microsoft’s Confidential consortium framework (CCF), which can be successfully audited regardless of how many replicas misbehave.
  * Worked with members of the CCF team and external customers to productize CCF. 
  * Designed and built a distributed system that executes machine learning inference requests in an untrusted environment. This system utilizes a novel Byzantine fault tolerant consensus protocol to provide users confidence in the validity of the inference results.
  
* Senior Research Software Engineer, Microsoft Research, 2015 - 2019
  * FaRM and A1 are a distributed transactional in-memory storage system and distributed graph database which allow micro-second remote memory reads.
  * Designed, built, and productized FaRM and A1, which were deployed as part of the Bing search engine.
  * Designed and built a low latency distributed time service with micro-second precision.
  * Built a hybrid file system that utilizes non-volatile memory and SSDs to provide highly performant reads and writes while at the same time reducing SSD wear.
  * Integrated the previously mentioned file system with Microsoft’s FaRM. This feature reduced the storage overheads, ultimately decreasing the cost of deploying FaRM in a production environment by two thirds.
  * Designed and implemented a framework to allow users of FaRM to write code that can efficiently run on the same servers as FaRM replicas. Implemented a lock-free IPC and process management mechanism to support low latency communication between user processes and a FaRM replica.

* Member of Technical Staff, Microsoft Research, 2014 - 2015
  * Designed and built an in-memory distributed storage system which utilizes RDMA for communication to allow for low latency operations
  * Designed and build a lock free memory allocator, that can support either RDMA or CPU atomic operations
  * Implemented and designed a distributed key-value store on top of distributed memory
  * Implemented the distributed logging infrastructure for extremely high volume mobile applications

* Software Engineer II, Cosmos Distributed Storage, Microsoft, 2011 - 2014
  * The Cosmos distributed storage team is responsible for developing and maintaining a store that contains over an exabyte of data.
  * Designed and built an application which stores arbitrary data on SSD using a specialized on-disk layout. This allows for low read/write latency and high throughput while minimizing write amplification on top of NTFS.
  * Participated in the design and development of the next generation control plane architecture for Cosmos storage
  * Implemented features to increase data throughput, reduce latencies, and increase the number of nodes in a Cosmos environment
  * Operated the Cosmos storage system and resolved customer escalations
  * Designed and established new development and validation methodologies ranging from integrating new testing frameworks to automating manual processes

* Software Engineer, Cosmos Distributed Execution, Microsoft, 2009- 2011
  * The Cosmos distributed execution team is responsible for designing, developing, and advancing a distributed scheduling system.
  * Designed and developed testing strategies for validating core distributed execution components, the primary of which is a distributed execution system - an evolution of Microsoft Research’s Dryad
  * Drove the testing strategy for a component that is the single execution scheduling point for a cluster of tens of thousands of machines by developing monitoring, reporting, and replay/simulation applications
  * Designed and developed a data ingestion and processing pipeline which consistently validates metrics of the batch job execution engine

* Software Engineer Intern, Cosmos Distributed Execution, Microsoft, 2008 - 2009
  * Created and executed a validation strategy for a multi-tiered distributed cache

* Software Developer, Tango Technology, Sydney Australia, 2006 - 2008
  * Designed and developed a distributed trading execution system for RARA Investment Limited using Microsoft technologies (C#, SQL Server, Windows Sockets, etc.), IRESS, and Bloomberg
  * Developed websites and reporting tools using Microsoft technologies (C#, SQL Server, Excel, etc.) for financial firms

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed  %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>

Patents
======
* Erasure coding of data within a group of storage units based on connection characteristics (with Robert Jenkins, Edmund Nightingale, Cheng Huang, Parikshit Gopalan, and Sergey Yekhanin)
  * Patent Issued, number 9,983,959
* File storage system including tiers (with Edmund Nightingale, Pavan Edara, and Mugdha Jamsandekar)
  * Patent Issued, number 9,824,092
* Fast read/write between networked computers via RDMA-based RPC requests (with Yutaka Suzue)
  * Patent Issued, number 9,792,248
* Low latency RDMA-based distributed storage (with Yutaka Suzue and Knut Risvik)
  * Patent Issued, number 10,375,167
* Clock Synchronization (with Miguel Castro, Richie Rhanna, Dushyanth Narayanan, Aleksandar Dragojevic, Matthew Renzelmann, Anders Gjerdrum, Stanko Novakovic, and Georgios Chatzopoulos)
  * Patent Issued, number 10,613,578
* Distributed self-directed lock-free RDMA-based b-tree key-value manager (with Yutaka Suzue)
  * Patent Issued, number 10,713,210 
* Distributed lock-free RDMA-based memory allocation and de-allocation (with Yutaka Suzue and Knut Risvik)
  * Patent Issued, number 10,725,963
* Distributed Graph Databases (with Knut Mange Risvik, Chiranjeeb Buranohain, Richie Khanna, Tim Tan, Matthew Renzelmann, Ming-Chuan Wu, Miguel Castro, Dushyanth Narayanan, and Aleksandar Dragojevic)
  * Patent Issued, number 10,810,179 
* Performing transactions in distributed transactional memory systems (with Miguel Castro, Richie Rhanna, Dushyanth Narayanan, Aleksandar Dragojevic, Matthew Renzelmann, Anders Gjerdrum, Stanko Novakovic, and Georgios Chatzopoulos)
  * Patent Issued, number 10,929,376
* Side-Channel Protection (with Sylvan Clebsch and Felix Schuster)
  * Patent filed 2019
* Receipts in a Distributed Ledger (with Eddy Ashton, Miguel Castro, Amaury Chamauyou, Sylvan Clebsch, Antoine Delignat-Lavaud, Cedric Fournet, Julien Maffre, and Peter Pietzuch)
  * Patent filed 2021
* Enclave Cloning (with Yoshimichi Nakatsuka, Ercan Ozturk, Andrew Paverd, and Peter Pietzuch)
  * Patent filed 2021