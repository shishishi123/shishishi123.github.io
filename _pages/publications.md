---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
## 2024
- Hexuan Yu, **Shanghao Shi**, Yi Shi, Eric Burger, Y. Thomas Hou, and Wenjing Lou. "Pri-Share: Enabling Inter-SAS Privacy Protection via Secure Multi-Party Spectrum Allocation." In 2024 IEEE International Symposium on Dynamic Spectrum Access Networks (DySPAN 24). (to appear) [[PDF]](http://shishishi123.github.io/files/sas-privacy.pdf)
- **Shanghao Shi**, Yang Xiao, Changlai Du, Yi Shi, Chonggang Wang, Robert Gazda, Y. Thomas Hou, Eric Burger, Luiz DaSilva, and Wenjing Lou. 2024. "TriSAS: Toward Dependable Inter-SAS Coordination with Auditability." In ACM Asia Conference on Computer and Communications Security (ASIA CCS’24), July 1–5, 2024, Singapore, Singapore. ACM, New York, NY, USA, 13 pages. https://doi.org/10.1145/3634737.3645005 [[PDF]](http://shishishi123.github.io/files/trisas.pdf)

## 2023
- Chaoyu Zhang, Ning Wang, **Shanghao Shi**, Changlai Du, Wenjing Lou, and Y. Thomas Hou. "MINDFL: Mitigating the Impact of Imbalanced and Noisy-labeled Data in Federated Learning with Quality and Fairness-Aware Client Selection." In 2023 IEEE Military Communications Conference (MILCOM 23), pp. 331-338. IEEE, 2023. [[PDF]](http://shishishi123.github.io/files/mindfl.pdf)
- Shaoyu Li, **Shanghao Shi**, Yang Xiao, Chaoyu Zhang, Y. Thomas Hou, and Wenjing Lou. "Bijack: Breaking Bitcoin Network with TCP Vulnerabilities." In European Symposium on Research in Computer Security (ESORICS 23), pp. 306-326. Cham: Springer Nature Switzerland, 2023. [[PDF]](http://shishishi123.github.io/files/Bijack.pdf)
- Yang Xiao, **Shanghao Shi**, Wenjing Lou, Chonggang Wang, Xu Li, Ning Zhang, Y. Thomas Hou, and Jeffrey H. Reed. "BD-SAS: Enabling Dynamic Spectrum Sharing in Low-trust Environment." IEEE Transactions on Cognitive Communications and Networking (2023). [[PDF]](http://shishishi123.github.io/files/bdsas.pdf)
- **Shanghao Shi**, Yang Xiao, Changlai Du, Md Hasan Shahriar, Ao Li, Ning Zhang, Y. Thomas Hou, and Wenjing Lou. 2023. MS-PTP: Protecting Network Timing from Byzantine Attacks. In Proceedings of the 16th ACM Conference on Security and Privacy in Wireless and Mobile Networks (WiSec '23). Association for Computing Machinery, New York, NY, USA, 61–71. https://doi.org/10.1145/3558482.3590184 [[PDF]](http://shishishi123.github.io/files/msptp.pdf)

## Before
- Yang Xiao, **Shanghao Shi**, Wenjing Lou, Chonggang Wang, Xu Li, Ning Zhang, Y. Thomas Hou, and Jeffrey H. Reed. "Decentralized spectrum access system: Vision, challenges, and a blockchain solution." IEEE Wireless Communications 29, no. 1 (2022): 220-228. [[PDF]](http://shishishi123.github.io/files/decensas.pdf)
- **Shanghao Shi**, Yang Xiao, Wenjing Lou, Chonggang Wang, Xu Li, Y. Thomas Hou, and Jeffrey H. Reed. "Challenges and new directions in securing spectrum access systems." IEEE Internet of Things Journal 8, no. 8 (2021): 6498-6518. [[PDF]](http://shishishi123.github.io/files/spectrumsurvey.pdf)
- Yang Xiao, **Shanghao Shi**, Ning Zhang, Wenjing Lou, and Y. Thomas Hou. "Session key distribution made practical for CAN and CAN-FD message authentication." In Annual Computer Security Applications Conference (ACSAC 20), pp. 681-693. 2020. [[PDF]](http://shishishi123.github.io/files/cansecurity.pdf)

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

