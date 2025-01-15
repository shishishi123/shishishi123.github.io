---
title: "Protecting Network Timing from Byzantine Attacks within Time-Sensitive IoT Networks"
collection: research
permalink: /research/IoT-Security/
author_profile: true
---

## Research Problem
- Ensuring network time synchronization is super important for time-sensitive IoT networks such as 5G and automotive Ethernet because they have very stringent time synchronization requirements and failing to meet them (even for a millisecond-level desynchronization) can cause significant system performance degradation. 
- Technically, precision time protocol (PTP) is the widely-used network timing protocol that ensures time synchronization for many distributed networks.
- In this research, we first propose a powerful insider time shifting attack launched by a malicious PTP client that is able to gradually shift the system time of an arbitrarily chosen victim node, even when the network is protected by the existing authentication mechanisms.
- We verify the consequence of our attack on a real Turtlebot robotic platform demonstrating that the robots will go to the wrong trajectories when the attack is launched.
- As a countermeasure, we propose a multi-source time synchronization mechanism named MS-PTP that aggregates the timing measurements of multiple sources. We devise a Byzantine resilient aggregation mechanism, which can defend Byzantine timing attacks when less than one-third of the sources are affected and overcomes unavoidable benign noise during the timing measurement process.
- We provide a mathematical guarantee for the maximum error of our mechanism and validate the effectiveness of our mechanism on hardware testbeds.
