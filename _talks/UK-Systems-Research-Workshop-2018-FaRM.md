---
title: "FaRM and MVCC"
collection: talks
type: "Talk"
permalink: /talks/UK-Systems-Research-Workshop-2018-FaRM
venue: "UK Systems workshop 2018"
date: 2018-03-21
location: "Northumberland, United Kingdom"
---

FaRM is a main memory distributed computing platform that provides distributed transactions with strict serializability, high performance, durability, and high availability. FaRM’s transactional reads however, do not provide opacity. Transactions sometimes operate on inconsistent state before aborting, which can result in program crashes. Programmers using FaRM are required to introduce consistency checks, similar to the checks used in lock-free algorithms to prevent this. This is a major issue as it significantly complicates the programming model, even for the experience programmers that use FaRM to build production systems. To fix this problems, we have changed the FaRM protocols to provide opacity using Multiversion Concurrency Control (MVCC). -- [UK Systems Workshop](http://uksystems.org/workshop/2018/)
