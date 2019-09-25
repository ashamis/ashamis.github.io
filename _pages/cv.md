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
* B.S. in Computer Science, University of New South Wales, 2009
* B.S. in Mathematics, University of New South Wales, 2009
* Ph.D in Computing, Imperial College London, 2022 (expected)

Work experience
======
* Senior Research Software Development Engineer, Microsoft Research Cambridge, Confidential Computing, 2018 - Current
  
* Senior Research Software Development Engineer, Microsoft Research Cambridge, System and Networking, 2017 - 2018
  * Built a hybrid file system that utilizes non-volatile memory and SSDs to provide highly performant read and write APIs to the high-level system while at the same time reducing SSD wear
  * Integrated the previously mentioned file system with Microsoft’s FaRM, an in-memory transactional store; improved storage from three copies of data in memory with FaRM to one copy in memory and two on SSD. This change has allowed teams in Microsoft that use FaRM to reduce the financial impact of running FaRM.
  * Implemented innovative ways to reduce the amount of main memory needed to store metadata regarding objects that were written to SSD such that only two bytes plus a small static overhead are needed to find an object that is stored on disk
  * Created an initial proposal on how to extent FaRM to support geographically distributed transactions. Currently, working to consolidate the design with other FaRM team members.
  * Currently working with other members of the FaRM team in Microsoft Research Cambridge to submit a publication regarding FaRM’s implementation of MVCC to OSDI 2018. This involves performance debugging all aspects of FaRM to find code and design issues that affect the performance of the system.

* Senior Research Software Development Engineer, Microsoft Research NeXT, 2015 - 2017
  * As a member of the Farm/A1 team designed and built a distributed transactional memory storage system and distributed graph database.
  * Designed and implemented a framework to allow users of Farm to write code that can efficiently run either in the same process as FaRM
  * Built and designed a lock free IPC mechanism to support low latency communication between different processes on the same computer.
  * Added features and resolved issues in FaRM to contribute to making FaRM a production service in Microsoft.
  * Optimized the Zookeeper service for the FaRM SOSP 2015 publication

* Member of Technical Staff, Special Projects, Microsoft Research, 2014 - 2015
  * Designed and built an in-memory distributed storage system which utilizes RDMA for communication to allow for low latency operations
  * Designed and build a lock free memory allocator, that can support either RDMA or CPU atomic operations
  * Implemented and designed a distributed key-value store on top of distributed memory
  * Implemented the distributed logging infrastructure for extremely high volume mobile applications

* Software Design Engineer II, Cosmos Distributed Storage, Microsoft, 2011 - 2014
  * The Cosmos distributed storage team is responsible for developing and maintaining a store that contains over an exabyte of data.
  * Designed and built an application which stores arbitrary data on SSD using a specialized on-disk layout. This allows for low read/write latency and high throughput while minimizing write amplification on top of NTFS.
  * Participated in the design and development of the next generation control plane architecture for Cosmos storage
  * Implemented features to increase data throughput, reduce latencies, and increase the number of nodes in a Cosmos environment
  * Operated the Cosmos storage system and resolved customer escalations
  * Designed and established new development and validation methodologies ranging from integrating new testing frameworks to automating manual processes

* Software Design Engineer in Test, Cosmos Distributed Execution, Microsoft, 2009- 2011
  * The Cosmos distributed execution team is responsible for designing, developing, and advancing a distributed scheduling system.
  * Designed and developed testing strategies for validating core distributed execution components, the primary of which is a distributed execution system - an evolution of Microsoft Research’s Dryad
  * Drove the testing strategy for a component that is the single execution scheduling point for a cluster of tens of thousands of machines by developing monitoring, reporting, and replay/simulation applications
  * Designed and developed a data ingestion and processing pipeline which consistently validates metrics of the batch job execution engine

* Software Design Engineer in Test Intern, Cosmos Distributed Execution, Microsoft, 2008 - 2009
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
* Distributed lock-free RDMA-based memory allocation and de-allocation (with Yutaka Suzue and Knut Risvik)
  * Patent filed 2015
* Distributed self-directed lock-free RDMA-based b-tree key-value manager (with Yutaka Suzue)
  * Patent filed 2015
* Distributed Graph Databases (with Knut Mange Risvik, Chiranjeeb Buranohain, Richie Khanna, Tim Tan, Matthew Renzelmann, Ming-Chuan Wu, Miguel Castro, Dushyanth Narayanan, and Aleksandar Dragojevic)
  * Patent filed 2015
* Performing transactions in distributed transactional memory systems (with Miguel Castro, Richie Rhanna, Dushyanth Narayanan, Aleksandar Dragojevic, Matthew Renzelmann, Anders Gjerdrum, Stanko Novakovic, and Georgios Chatzopoulos)
  * Patent filed 2018
* Clock Synchronization (with Miguel Castro, Richie Rhanna, Dushyanth Narayanan, Aleksandar Dragojevic, Matthew Renzelmann, Anders Gjerdrum, Stanko Novakovic, and Georgios Chatzopoulos)
  * Patent filed 2018
* Side-Channel Protection (with Sylvan Clebsch and felix Schuster)
  * Patent filed 2019
