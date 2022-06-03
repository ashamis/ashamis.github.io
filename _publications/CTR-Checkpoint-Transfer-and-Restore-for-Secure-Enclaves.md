---
title: "CTR: Checkpoint, Transfer, and Restore for Secure Enclaves"
authors: "Yoshimichi Nakatsuka, Ercan Ozturk, <b>Alex Shamis</b>, Andrew Paverd, Peter Pietzuch"
collection: publications
permalink: /publication/CTR-Checkpoint-Transfer-and-Restore-for-Secure-Enclaves
excerpt: 'We present CTR, a software-only design to retrofit migration functionality into existing TEE architectures, whilst maintaining their expected security guarantees. Our design allows TEEs to be interrupted and migrated at arbitrary points in their execution, thus maintaining compatibility with existing VM and process migration techniques. By cooperatively involving the TEE in the migration process, our design also allows application developers to specify stateful migration-related policies, such as limiting the number of times a particular TEE may be migrated. Our prototype implementation for Intel SGX demonstrates that migration latency increases linearly with the size of the TEE memory and is dominated by TEE system operations.'
date: 2022-05-31
paperurl: 'https://arxiv.org/pdf/2205.15359.pdf'
venue: 'ArXiv'
---
Hardware-based Trusted Execution Environments (TEEs) are becoming increasingly prevalent in cloud computing, forming the basis for confidential computing. However, the security goals of TEEs sometimes conflict with existing cloud functionality, such as VM or process migration, because TEE memory cannot be read by the hypervisor, OS, or other software on the platform. Whilst some newer TEE architectures support migration of entire protected VMs, there is currently no practical solution for migrating individual processes containing in-process TEEs. The inability to migrate such processes leads to operational inefficiencies or even data loss if the host platform must be urgently restarted.

We present CTR, a software-only design to retrofit migration functionality into existing TEE architectures, whilst maintaining their expected security guarantees. Our design allows TEEs to be interrupted and migrated at arbitrary points in their execution, thus maintaining compatibility with existing VM and process migration techniques. By cooperatively involving the TEE in the migration process, our design also allows application developers to specify stateful migration-related policies, such as limiting the number of times a particular TEE may be migrated. Our prototype implementation for Intel SGX demonstrates that migration latency increases linearly with the size of the TEE memory and is dominated by TEE system operations.

[Download paper here](https://arxiv.org/pdf/2205.15359.pdf)
