---
layout: default
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

## Model Inversion Attacks against Secure Federated Learning Systems

## Research Background
- Federated learning (FL) is a distributed learning paradigm that enables its participants to collaboratively train machine learning models without sharing local datasets. In this context, it is considered as a *privacy-preserving* paradigm. 
- However, recent optimization-based model inversion attacks show that a curious server can reverse the shared model updates between FL participants back to local training samples, challenging this privacy guarantee. 
- To address this, a multi-party computation mechanism named *secure aggregation* is proposed, which hides individual model updates behind cryptographic masks but keeps the aggregated results identical to pre-masked values to keep system utility. This prevents the optimization-based attackers from obtaining individual model updates, effectively defending these attacks. 

<figure class="center">
<img src="https://github.com/shishishi123/shishishi123.github.io/blob/master/files/figures/ScaleMIA-ThreatModel.png" alt="drawing" width="350" height="350" />
<figcaption>Threat model for model inversion attacks in secure federated learning systems.</figcaption>
</figure>

## Our Mechanism
- In this research, we propose a more powerful model inversion attack named Scale-MIA that not only breaks the secure aggregation, but also significantly improves the attack efficiency and scalability.
- Our attack identifies the latent space as the key layer to breach the privacy and decompose the complex reconstruction problem into two steps including first reversing the aggregated model updates back to latent space representations (LSRs) via an attack module named linear leakage, and then reversing the LSRs back to local training samples via a fine-tuned decoder.
- Our attack only involves closed-form calculations, and thus is much more efficient than existing works. 
- Our attack challenges the fundamental privacy-preserving property of the federated learning systems, and calls for effective defense against such advanced attacks.

<figure class="center">
<img src="https://github.com/shishishi123/shishishi123.github.io/blob/master/files/figures/Attackflow.png" alt="drawing" height="450" />
<figcaption>Scale-MIA is a two-phase attack. The first phase is performed locally to produce essential information to conduct the second phase. The second is the actual attack phase, during which the attacker interacts with the clients and reconstructs their local training samples.</figcaption>
</figure>

## Experiment Results
- We implement our attack on popular machine learning models and datasets and the results show that our attack can reconstruct hundreds of local training samples simultaneously within a few seconds.

<figure class="center">
<img src="https://github.com/shishishi123/shishishi123.github.io/blob/master/files/figures/celeba_input_batch.png" alt="drawing" width="450" />
<img src="https://github.com/shishishi123/shishishi123.github.io/blob/master/files/figures/celeba_recovered_batch.png" alt="drawing" width="450" />
<figcaption>The comparison between the original images and the reconstructed images with batch size 64 on CelebA.</figcaption>
</figure>

{% for post in site.pages %}
{% include archive-single.html %}
{% endfor %}
