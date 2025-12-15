---
title: "TEE<sup>BFT</sup>: Pricing the Security of Data Center Execution Assurance"
authors: "<b>Alex Shamis</b>, Matt Stephenson, Linfeng Zhou"
collection: publications
permalink: /publication/TEE-BFT-Pricing-the-Security-of-Data-Center-Execution-Assurance
excerpt: 'Trusted Execution Environments (TEEs) are a promising mitigation because they allow a single trusted broker to interface securely with external systems. This paper develops a cost-of-collusion principal-agent model for compromising a TEE in a Data Center Execution Assurance design.'
date: 2025-10-30
paperurl: '/files/TEE-BFT-Pricing-the-Security-of-Data-Center-Execution-Assurance.pdf'
venue: 'Technical Report'
---
Blockchains face inherent limitations when communicating outside their own ecosystem, largely due to the Byzantine Fault Tolerant (BFT) 3f+1 security model. Trusted Execution Environments (TEEs) are a promising mitigation because they allow a single trusted broker to interface securely with external systems. This paper develops a cost-of-collusion principal-agent model for compromising a TEE in a Data Center Execution Assurance design. The model isolates the main drivers of attack profitability: a K-of-n coordination threshold, independent detection risk q, heterogeneous per-member sanctions F_i, and a short-window flow prize (omega) proportional to the value secured (beta times V). We derive closed-form deterrence thresholds and a conservative design bound (V_safe) that make collusion unprofitable under transparent parameter choices. Calibrations based on time-advantaged arbitrage indicate that plausible TEE parameters can protect on the order of one trillion dollars in value. The analysis informs the design of TEE-BFT, a blockchain architecture that combines BFT consensus with near-stateless TEEs, distributed key generation, and on-chain attestation to maintain security when interacting with external systems.

[Download paper here](/files/TEE-BFT-Pricing-the-Security-of-Data-Center-Execution-Assurance.pdf)

[Download BibTex here](/files/TEE-BFT-Pricing-the-Security-of-Data-Center-Execution-Assurance.bib)
