---
layout: toc
title : Browning Block Life - The Series

---
Seasons 1 through 3
{% assign episodes = site.bbl | where: "layout", "episode" %}


<ul class="episodes">
{% for post in episodes | reverse : "episode" %}
  <li>
    <a href="{{ post.url }}">
      <img src="/assets/bbl/bbl-thumb-{{post.season}}-{{post.episode}}.jpg" class="thumbnail">
      <span>{{ post.title }}</span>
    </a>
    <p>Season {{post.season}} - Episode {{post.episode}} | {{post.duration}} min</p>
  </li>
{% endfor %}
</ul>
