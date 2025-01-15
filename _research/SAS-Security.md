---
title: "Building Trustworthy and Verifiable Spectrum Sharing Systems."
collection: research
permalink: /research/SAS-Security/
author_profile: true
---

## Research Problem

- To address spectrum scarcity in 5G, the FCC and NTIA opened the 3.55GHz-3.7GHz band for shared use among military and commercial users under a three-tiered access model, in which military users have the highest priority to gain spectrum resources on demand, and commercial users locate at lower two layers utilizing spectrum resources when available.


- Seven entities, including Google and Federated Wireless, manage the shared band via their own Spectrum Access System (SAS) servers. However, the lack of coordination among these entities risks allocation conflicts and service disruption.



- In this research, we propose a fault-tolerant, verifiable, and efficient inter-SAS coordination mechanism named TriSAS.
- We leverage the blockchain database as the fundamental backbone to store all records in the transactions, where each SAS serves as a blockchain node.
- We decompose the coordination problem into two phases including input synchronization and decision finialization. The first phase ensures all SAS share the same input set. The second phase consists of three subphases including generating, voting, and finalizing, in which all SAS produce their own spectrum proposals locally, and then vote and finalize one with the best evaluation score.
- Our mechanism ensures that all honest SAS finalize the same spectrum proposal when malicious nodes are less than one-third of the total population.

## Results
- We implement our mechanism on a distributed network across the U.S. continent and the results show that our proposed system achieves high throughput and low latency.
