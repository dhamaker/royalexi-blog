---
layout: toc
title : Browning Block Life

---
{% assign episodes = site.bbl | where: "layout", "episode" %}
<ul class="posts">
{% for post in episodes | reverse : "episode" %}
<li class=""><a href="{{ post.url }}">{{ post.title }}</a> Season {{post.season}} Episode {{post.episode}}.  Duration {{post.duration}}
</li>
{% endfor %}
</ul>
