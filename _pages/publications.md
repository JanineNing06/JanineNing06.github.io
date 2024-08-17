---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

Lists of Publication
======
* Zimu Xu, Wei Tian, Yingxin Liu, **Wanjun Ning** and Jingjin Wu, “A Ring Topology-Based Communication-Efficient Scheme for D2D Wireless Federated Learning,” *In 2023 IEEE Global Communications Conference (GLOBECOM)*, 2023, pp. 2820-2825. [Paper](https://ieeexplore.ieee.org/abstract/document/10437407)
* **Wanjun Ning**, Zimu Xu, Jingjin Wu and Tiejun Tong, “Sequence Q-Learning Algorithm for Optimal Mobility-Aware User Association,” *In 2022 IEEE International Conference on Communications (ICC)*, 2022, pp. 726-732. [Paper](https://ieeexplore.ieee.org/abstract/document/9838645)
