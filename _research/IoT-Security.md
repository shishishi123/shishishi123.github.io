---
title: "Protecting Network Timing from Byzantine Attacks within Time-Sensitive IoT Networks"
collection: research
permalink: /research/IoT-Security/
author_profile: true
---

## Research Problem
- Ensuring *network time synchronization* is super important for time-sensitive IoT networks such as 5G and automotive Ethernet because they have very stringent time synchronization requirements and failing to meet them (even for a millisecond-level desynchronization) can cause significant system performance degradation. 
- Technically, *precision time protocol (PTP)* is the widely-used network timing protocol that ensures time synchronization for many distributed networks.

<figure style="display: flex; flex-direction: column; align-items: center; text-align: center; margin: auto;">
  <img src="https://raw.githubusercontent.com/shishishi123/shishishi123.github.io/refs/heads/master/files/figures/PTP-Testbed.png" 
       alt="Testbed" 
       style="width:550px; height:auto; display: block; margin: auto;" />
  <figcaption style="caption-side: bottom; text-align: center; margin-top: 10px;">
    PTP Testbed.
  </figcaption>
</figure>

- In this research, we first propose a powerful insider time shifting attack launched by a malicious PTP client that is able to gradually shift the system time of an arbitrarily chosen victim node, even when the network is protected by the existing authentication mechanisms.
- 
<figure style="display: flex; flex-direction: column; align-items: center; text-align: center; margin: auto;">
  <img src="https://raw.githubusercontent.com/shishishi123/shishishi123.github.io/refs/heads/master/files/figures/Attack-Results.png" 
       alt="Attack Results" 
       style="width:1550px; height:auto; display: block; margin: auto;" />
  <figcaption style="caption-side: bottom; text-align: center; margin-top: 10px;">
    Time shifting attack results over PTP implementation PTPD and LinuxPTP. The overall trend shows the effective manipulation of the victim clock offset.
  </figcaption>
</figure>

- As a countermeasure, we propose a multi-source time synchronization mechanism named MS-PTP that aggregates the timing measurements of multiple sources. We devise a Byzantine resilient aggregation mechanism, which can defend Byzantine timing attacks when less than one-third of the sources are affected and overcomes unavoidable benign noise during the timing measurement process.
- We provide a mathematical guarantee for the maximum error of our mechanism and validate the effectiveness of our mechanism on hardware testbeds.

## Results
- We verify the consequence of our attack on a real Turtlebot robotic platform demonstrating that the robots will go to the wrong trajectories when the attack is launched.

<figure style="display: flex; flex-direction: column; align-items: center; text-align: center; margin: auto;">
  <img src="https://raw.githubusercontent.com/shishishi123/shishishi123.github.io/refs/heads/master/files/figures/Robotic-Attack-Results.png" 
       alt="Robotic Attack Results" 
       style="width:500px; height:auto; display: block; margin: auto;" />
  <figcaption style="caption-side: bottom; text-align: center; margin-top: 10px;">
    The consequence of de-synchronization attack on Turtlebot3.
  </figcaption>
</figure>

- We implement our defense mechanism on our PTP harware testbed and the results show that our proposed defense can effectively defense various timing attacks.
- Our mechanism is compatible with the current indistrial PTP standard.

<figure style="display: flex; flex-direction: column; align-items: center; text-align: center; margin: auto;">
  <img src="https://raw.githubusercontent.com/shishishi123/shishishi123.github.io/refs/heads/master/files/figures/Defense-Performance.png" 
       alt="Defense Performance" 
       style="width:650px; height:auto; display: block; margin: auto;" />
  <figcaption style="caption-side: bottom; text-align: center; margin-top: 10px;">
    MS-PTP accuracy performance under attack (𝑐𝑢 – cumulative delay, 𝑐𝑠 – constant delay, 𝑟𝑑 – random delay).
  </figcaption>
</figure>

## Reference
- **Shanghao Shi**, Yang Xiao, Changlai Du, Md Hasan Shahriar, Ao Li, Ning Zhang, Y. Thomas Hou, and Wenjing Lou. 2023. MS-PTP: Protecting Network Timing from Byzantine Attacks. In Proceedings of the 16th ACM Conference on Security and Privacy in Wireless and Mobile Networks (**WiSec 23**). Association for Computing Machinery, New York, NY, USA, 61–71. [[PDF]](http://shishishi123.github.io/files/msptp.pdf)






