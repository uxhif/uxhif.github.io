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

My research focuses on geometric deep learning. More broadly, I am interested in understanding the theoretical structure of deep learning models and enhancing their learning efficiency and generalization through mathematical frameworks, including geometry, algebra, and topology. I am particularly interested in developing principled learning frameworks that achieve strong model generality grounded in mathematical theory.

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
