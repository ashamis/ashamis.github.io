---
title: "Dropbear: Machine Learning Marketplaces made Trustworthy with Byzantine Model Agreement"
authors: "<b>Alex Shamis</b>, Peter Pietzuch, Antoine Delignat-Lavaud, Andrew Paverd, Manuel Costa"
collection: publications
permalink: /publication/Dropbear-Machine-Learning-Marketplaces-made-Trustworthy-with-Byzantine-Model-Agreement
excerpt: 'Marketplaces for machine learning (ML) models are emerging as a way for organizations to monetize models. They allow model owners to retain control over hosted models by using cloud resources to execute ML inference requests for a fee, preserving model confidentiality. Clients that rely on hosted models require trustworthy inference results, even when models are managed by third parties. While the resilience and robustness of inference results can be improved by combining multiple independent models, such support is unavailable in today's marketplaces.'
date: 2022-05-31
paperurl: 'https://arxiv.org/pdf/2205.15757.pdf'
venue: 'ArXiv'
---
Marketplaces for machine learning (ML) models are emerging as a way for organizations to monetize models. They allow model owners to retain control over hosted models by using cloud resources to execute ML inference requests for a fee, preserving model confidentiality. Clients that rely on hosted models require trustworthy inference results, even when models are managed by third parties. While the resilience and robustness of inference results can be improved by combining multiple independent models, such support is unavailable in today's marketplaces.
<\br>
<\br>
We describe Dropbear, the first ML model marketplace that provides clients with strong integrity guarantees by combining results from multiple models in a trustworthy fashion. Dropbear replicates inference computation across a model group, which consists of multiple cloud-based GPU nodes belonging to different model owners. Clients receive inference certificates that prove agreement using a Byzantine consensus protocol, even under model heterogeneity and concurrent model updates. To improve performance, Dropbear batches inference and consensus operations separately: it first performs the inference computation across a model group, before ordering requests and model updates. Despite its strong integrity guarantees, Dropbear's performance matches that of state-of-the-art ML inference systems: deployed across 3 cloud sites, it handles 800 requests/s with ImageNet models.
Permissioned ledger systems allow a consortium of members that do not trust one another to execute transactions safely on a set of replicas. Such systems typically use Byzantine fault tolerance (BFT) protocols to distribute trust, which only ensures safety when fewer than 1/3 of the replicas misbehave. Providing guarantees beyond this threshold is a challenge: current systems assume that the ledger is corrupt and fail to identify misbehaving replicas or hold the members that operate them accountable---instead all members share the blame.

[Download paper here](https://arxiv.org/pdf/2205.15757.pdf)
