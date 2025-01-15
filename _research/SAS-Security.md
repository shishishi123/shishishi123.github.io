---
title: "Building Trustworthy and Verifiable Spectrum Sharing Systems."
collection: research
permalink: /research/SAS-Security/
author_profile: true
---

## Research Problem

- To address spectrum scarcity in 5G, the FCC and NTIA opened the 3.55GHz-3.7GHz band for shared use among military and commercial users under a three-tiered access model, in which military users have the highest priority to gain spectrum resources on demand, and commercial users locate at lower two layers utilizing spectrum resources when available.

<figure style="display: flex; flex-direction: column; align-items: center; text-align: center; margin: auto;">
  <img src="https://raw.githubusercontent.com/shishishi123/shishishi123.github.io/refs/heads/master/files/figures/Three-tier-access.png" 
       alt="Three tier access model" 
       style="width:700px; height:auto; display: block; margin: auto;" />
  <figcaption style="caption-side: bottom; text-align: center; margin-top: 10px;">
    Three-tier spectrum access system for the 3.55GHz-3.7GHz CBRS band.
  </figcaption>
</figure>

- Seven entities, including Google and Federated Wireless, manage the shared band via their own Spectrum Access System (SAS) servers. However, the lack of coordination among these entities risks allocation conflicts and service disruption.

<figure style="display: flex; flex-direction: column; align-items: center; text-align: center; margin: auto;">
  <img src="https://raw.githubusercontent.com/shishishi123/shishishi123.github.io/refs/heads/master/files/figures/SAS-SystemModel.png" 
       alt="SAS system model" 
       style="width:750px; height:auto; display: block; margin: auto;" />
  <figcaption style="caption-side: bottom; text-align: center; margin-top: 10px;">
    Spectrum Access System (SAS) system model. Each SAS administrator owns and manages their own customers and services.
  </figcaption>
</figure>

- In this research, we propose a fault-tolerant, verifiable, and efficient inter-SAS coordination mechanism named TriSAS.
- We leverage the blockchain database as the fundamental backbone to store all records in the transactions, where each SAS serves as a blockchain node.
- We decompose the coordination problem into two phases including input synchronization and decision finialization. The first phase ensures all SAS share the same input set. The second phase consists of three subphases including generating, voting, and finalizing, in which all SAS produce their own spectrum proposals locally, and then vote and finalize one with the best evaluation score.
- Our mechanism ensures that all honest SAS finalize the same spectrum proposal when malicious nodes are less than one-third of the total population.

<figure style="display: flex; flex-direction: column; align-items: center; text-align: center; margin: auto;">
  <img src="https://raw.githubusercontent.com/shishishi123/shishishi123.github.io/refs/heads/master/files/figures/TriSAS-WorkFlow.png" 
       alt="TriSAS workflow" 
       style="width:1000px; height:auto; display: block; margin: auto;" />
  <figcaption style="caption-side: bottom; text-align: center; margin-top: 10px;">
    TriSAS workflow. The proposed mechanism involves two phases including the input synchronization phase and the decision finalization phase.
  </figcaption>
</figure>

## Results
- We implement our mechanism on a distributed network across the U.S. continent and the results show that our proposed system achieves high throughput and low latency.

<figure style="display: flex; flex-direction: column; align-items: center; text-align: center; margin: auto;">
  <img src="https://raw.githubusercontent.com/shishishi123/shishishi123.github.io/refs/heads/master/files/figures/Input-Sync-Results.png" 
       alt="Input sync results" 
       style="width:1250px; height:auto; display: block; margin: auto;" />
  <figcaption style="caption-side: bottom; text-align: center; margin-top: 10px;">
    Input synchronization throughput and latency performance. When n={4, 7, 10, 13}, the system can tolerate {1, 2, 3, 4} Byzantine faults.
  </figcaption>
</figure>

<figure style="display: flex; flex-direction: column; align-items: center; text-align: center; margin: auto;">
  <img src="https://raw.githubusercontent.com/shishishi123/shishishi123.github.io/refs/heads/master/files/figures/Decision-Final-Results.png" 
       alt="Decision final results" 
       style="width:1250px; height:auto; display: block; margin: auto;" />
  <figcaption style="caption-side: bottom; text-align: center; margin-top: 10px;">
    Decision finalization latency performance. When n={4, 7, 10, 13}, the system can tolerate {1, 2, 3, 4} Byzantine faults.
  </figcaption>
</figure>

## Reference
- **Shanghao Shi**, Yang Xiao, Changlai Du, Yi Shi, Chonggang Wang, Robert Gazda, Y. Thomas Hou, Eric Burger, Luiz DaSilva, and Wenjing Lou. 2024. "TriSAS: Toward Dependable Inter-SAS Coordination with Auditability." In ACM Asia Conference on Computer and Communications Security (**ASIA CCS 24**), July 1–5, 2024, Singapore, Singapore. ACM, New York, NY, USA, 13 pages. [[PDF]](http://shishishi123.github.io/files/trisas.pdf)
- Hexuan Yu, **Shanghao Shi**, Yi Shi, Eric Burger, Y. Thomas Hou, and Wenjing Lou. "Pri-Share: Enabling Inter-SAS Privacy Protection via Secure Multi-Party Spectrum Allocation." In 2024 IEEE International Symposium on Dynamic Spectrum Access Networks (**DySPAN 24**), Washington, DC, USA, 2024, pp. 347-356. [[PDF]](http://shishishi123.github.io/files/sas-privacy.pdf)
- Yang Xiao, **Shanghao Shi**, Wenjing Lou, Chonggang Wang, Xu Li, Ning Zhang, Y. Thomas Hou, and Jeffrey H. Reed. "BD-SAS: Enabling Dynamic Spectrum Sharing in Low-trust Environment." IEEE Transactions on Cognitive Communications and Networking (**TCCN 23**), vol. 9, no. 4, pp. 842-856, Aug. 2023. [[PDF]](http://shishishi123.github.io/files/bdsas.pdf)
- Yang Xiao, **Shanghao Shi**, Wenjing Lou, Chonggang Wang, Xu Li, Ning Zhang, Y. Thomas Hou, and Jeffrey H. Reed. "Decentralized spectrum access system: Vision, challenges, and a blockchain solution." IEEE Wireless Communications 29, no. 1 (**WCM 22**): 220-228. [[PDF]](http://shishishi123.github.io/files/decensas.pdf)
- **Shanghao Shi**, Yang Xiao, Wenjing Lou, Chonggang Wang, Xu Li, Y. Thomas Hou, and Jeffrey H. Reed. "Challenges and new directions in securing spectrum access systems." IEEE Internet of Things Journal 8, no. 8 (**IoT-J 21**): 6498-6518. [[PDF]](http://shishishi123.github.io/files/spectrumsurvey.pdf)




