---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

## 2023
- Shaoyu Li, **Shanghao Shi**, Yang Xiao, Chaoyu Zhang, Y. Thomas Hou, and Wenjing Lou. "Bijack: Breaking Bitcoin Network with TCP Vulnerabilities." In European Symposium on Research in Computer Security (ESORICS 23), pp. 306-326. Cham: Springer Nature Switzerland, 2023.
- Yang Xiao, **Shanghao Shi**, Wenjing Lou, Chonggang Wang, Xu Li, Ning Zhang, Y. Thomas Hou, and Jeffrey H. Reed. "BD-SAS: Enabling Dynamic Spectrum Sharing in Low-trust Environment." IEEE Transactions on Cognitive Communications and Networking (2023). [[PDF]](http://shishishi123.github.io/files/bdsas.pdf)
- **Shanghao Shi**, Yang Xiao, Changlai Du, Md Hasan Shahriar, Ao Li, Ning Zhang, Y. Thomas Hou, and Wenjing Lou. 2023. MS-PTP: Protecting Network Timing from Byzantine Attacks. In Proceedings of the 16th ACM Conference on Security and Privacy in Wireless and Mobile Networks (WiSec '23). Association for Computing Machinery, New York, NY, USA, 61–71. https://doi.org/10.1145/3558482.3590184 [[PDF]](http://shishishi123.github.io/files/msptp.pdf)

## Before

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

