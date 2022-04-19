---
title: "IA-CCF: Individual Accountability for Permissioned Ledgers"
authors: "<b>Alex Shamis</b>, Peter Pietzuch, Burcu Canakci, Miguel Castro, Cedric Fournet, Edward Ashton, Amaury Chamayou, Sylvan Clebsch, Antoine Delignat-Lavaud, Matthew Kerner, Julien Maffre, Olga Vrousgou, Christoph M. Wintersteiger, Manuel Costa, Mark Russinovich"
collection: publications
permalink: /publication/pac-practical-accountability-for-ccf
excerpt: 'We describe IA-CCF, a new permissioned ledger system that provides individual accountability. It can assign blame to the individual members that operate misbehaving replicas regardless of the number of misbehaving replicas or members. IA-CCF achieves this by signing and logging BFT protocol messages in the ledger, and by using Merkle trees to provide clients with succinct, universally-verifiable receipts as evidence of successful transaction execution. Anyone can audit the ledger against a set of receipts to discover inconsistencies and identify replicas that signed contradictory statements. IA-CCF also supports changes to consortium membership and replicas by tracking signing keys using a sub-ledger of governance transactions. IA-CCF provides strong disincentives to misbehavior with low overhead: it executes 47,000 tx/s while providing clients with receipts in two network round trips.'
date: 2022-04-06
paperurl: 'https://www.usenix.org/system/files/nsdi22-paper-shamis.pdf'
venue: 'Symposium on Networked Systems Design and Implementation (NSDI)'
---

Permissioned ledger systems allow a consortium of members that do not trust one another to execute transactions safely on a set of replicas. Such systems typically use Byzantine fault tolerance (BFT) protocols to distribute trust, which only ensures safety when fewer than 1/3 of the replicas misbehave. Providing guarantees beyond this threshold is a challenge: current systems assume that the ledger is corrupt and fail to identify misbehaving replicas or hold the members that operate them accountable---instead all members share the blame.

We describe IA-CCF, a new permissioned ledger system that provides individual accountability. It can assign blame to the individual members that operate misbehaving replicas regardless of the number of misbehaving replicas or members. IA-CCF achieves this by signing and logging BFT protocol messages in the ledger, and by using Merkle trees to provide clients with succinct, universally-verifiable receipts as evidence of successful transaction execution. Anyone can audit the ledger against a set of receipts to discover inconsistencies and identify replicas that signed contradictory statements. IA-CCF also supports changes to consortium membership and replicas by tracking signing keys using a sub-ledger of governance transactions. IA-CCF provides strong disincentives to misbehavior with low overhead: it executes 47,000 tx/s while providing clients with receipts in two network round trips.

[Download paper here](https://www.usenix.org/system/files/nsdi22-paper-shamis.pdf)
