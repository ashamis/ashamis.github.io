---
title: "DTAB: Distributing Trust Without Sharing Blame"
authors: "<b>Alex Shamis</b>, Peter Pietzuch, Burcu Canakci, Miguel Castro, Edward Ashton, Amaury Chamayou, Sylvan Clebsch, Antoine Delignat-Lavaud, Cedric Fournet, Matthew Kerner, Julien Maffre, Olga Vrousgou, Christoph M. Wintersteiger, Manuel Costa, Mark Russinovich"
collection: publications
permalink: /publication/pac-practical-accountability-for-ccf
excerpt: 'Permissioned ledger systems execute transactions on a set of replicas governed by members of a consortium. They use Byzantine fault tolerance protocols to distribute trust among the replicas, and thus can ensure linearizability if fewer than 1/3 of the replicas misbehave. With more misbehaving replicas, current systems provide no guarantees, and all replicas and members share the blame.

We describe PAC, a permissioned ledger system that assigns blame to misbehaving replicas while supporting governance transactions to change the consortium membership and the set of replicas. PAC signs and stores protocol messages in the ledger and provides clients with signed, universally-verifiable receipts as evidence that a transaction executed at a certain ledger position. If clients obtain a sequence of receipts that violate linearizability, anyone can audit the ledger and the sequence of receipts to assign blame to at least 1/3 of the replicas, even if all replicas and members misbehave. Auditing assigns blame by finding contradictory statements signed by the same replica. Since the set of replicas changes, PAC determines the valid signing keys at any point in the ledger using a shorter sub-ledger of governance transactions. PAC provides a strong disincentive to misbehavior at low cost: it can execute more than 48,000 transactions per second, and clients receive receipts in two network round trips.'
date: 2022-04-06
paperurl: 'https://arxiv.org/abs/2105.13116'
venue: 'Symposium on Networked Systems Design and Implementation (NSDI)'
---

Permissioned ledger systems execute transactions on a set of replicas governed by members of a consortium. They use Byzantine fault tolerance protocols to distribute trust among the replicas, and thus can ensure linearizability if fewer than 1/3 of the replicas misbehave. With more misbehaving replicas, current systems provide no guarantees, and all replicas and members share the blame.

We describe PAC, a permissioned ledger system that assigns blame to misbehaving replicas while supporting governance transactions to change the consortium membership and the set of replicas. PAC signs and stores protocol messages in the ledger and provides clients with signed, universally-verifiable receipts as evidence that a transaction executed at a certain ledger position. If clients obtain a sequence of receipts that violate linearizability, anyone can audit the ledger and the sequence of receipts to assign blame to at least 1/3 of the replicas, even if all replicas and members misbehave. Auditing assigns blame by finding contradictory statements signed by the same replica. Since the set of replicas changes, PAC determines the valid signing keys at any point in the ledger using a shorter sub-ledger of governance transactions. PAC provides a strong disincentive to misbehavior at low cost: it can execute more than 48,000 transactions per second, and clients receive receipts in two network round trips.

[Download paper here](https://arxiv.org/pdf/2105.13116)

[Download BibTex here](https://scholar.googleusercontent.com/scholar.bib?q=info:3ZSO78UgMLkJ:scholar.google.com/&output=citation&scisdr=CgXs4J7KEPeV50riMFs:AAGBfm0AAAAAYMzkKFu29JOtru54aEqHNwpdPk3w5Sli&scisig=AAGBfm0AAAAAYMzkKDSpx4-Dz7OuY8Uezr0TUY1iUFpK&scisf=4&ct=citation&cd=-1&hl=en)
