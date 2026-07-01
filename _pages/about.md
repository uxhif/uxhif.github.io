---
permalink: /
title: "Jiyun Park"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am Jiyun Park, a M.S. student at the [VLLab](https://vllab.kaist.ac.kr/) at KAIST in Daejeon, South Korea, under the supervision of [Prof. Seunghoon Hong](https://maga33.github.io/). 
Before this, I earned my B.S. degree from KAIST, majoring in Mathematical Sciences with a double major in Computer Science.

My research interests lie in the mathematical foundations of deep learning and the study of abstract structures underlying learning systems.
I aim to understand how neural networks form and organize representations, and how fundamental mathematical concepts such as geometry, topology, algebra, and symmetry can be used to describe the mechanisms behind learning, generalization, and abstraction. In particular, I am interested in the structural properties of neural representations, latent spaces, and foundation models, with the goal of developing theoretical frameworks that provide a principled understanding of modern AI systems.


News
-----
<ul>
  {% for item in site.data.news limit:5 %}
    <li>
      <strong>[{{ item.date | date: "%Y.%m" }}]</strong>
      {{ item.text }}
    </li>
  {% endfor %}
</ul>

Selected Publications
-----
{% assign pubs = site.publications | sort: "date" | reverse %}
<ul>
  {% for pub in pubs limit:5 %}
    <li>
      <strong>{{ pub.title }}</strong><br/>
      {{ pub.authors }}<br/>
      <em>{{ pub.venue }}</em>, {{ pub.date | date: "%Y" }}
      {% if pub.paperurl %}
        [<a href="{{ pub.paperurl }}">paper</a>]
      {% endif %}
    </li>
  {% endfor %}
</ul>

<p>
  <a href="/publications/">See more →</a>
</p>

<!--Example: editing a Markdown file for a talk
![Editing a Markdown file for a talk](/images/editing-talk.png)-->
