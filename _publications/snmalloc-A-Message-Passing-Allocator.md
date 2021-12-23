---
title: "snmalloc: A Message Passing Allocator"
authors: "Paul Liétar, Theodore Butler, Sylvan Clebsch, Sophia Drossopoulou, Juliana Franco, Matthew J. Parkinson, <b>Alex Shamis</b>, Christoph M. Wintersteiger, David Chisnall"
collection: publications
permalink: /publication/snmalloc-A-Message-Passing-Allocator
excerpt: 'This paper presents snmalloc, a new point in the allocator/deallocator design space. Instead of thread-caching, we use lightweight lock-free message-passing to send batches of deallocations to the originating thread.'
date: 2019-06-23
paperurl: '/files/snmalloc-A-Message-Passing-Allocator.pdf'
venue: '2019 ACM SIGPLAN International Symposium on Memory Management (ISMM)'
---

Snmalloc is an implementation of malloc aimed at workloads in which objects are typically deallocated by a different thread than the one that had allocated them. We use the term producer/consumer for such workloads. Snmalloc uses a novel message passing scheme which returns deallocated objects to the originating allocator in batches without taking any locks. It also uses a novel bump pointer-free list data structure with which just 64-bits of meta-data are sufficient for each 64 KiB slab. On such producer/consumer benchmarks our approach performs better than existing allocators.

Snmalloc is available at [https://github.com/Microsoft/snmalloc](https://github.com/Microsoft/snmalloc).

[Download paper here](/files/snmalloc-A-Message-Passing-Allocator.pdf)

[Download BibTex here](/files/snmalloc-A-Message-Passing-Allocator.bib)
