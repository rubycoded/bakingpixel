---
layout: page
title: Tag archive
permalink: /tags/
---

Click on a tag to see relevant list of posts.

<ul class="tags">
{% for tag in site.tags %}
  {% assign t = tag | first %}
  <li><a href="/tags/#{{t | downcase | replace:" ","-" }}">{{ t | downcase }}</a></li>
{% endfor %}
</ul>

---

{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}

<h2 class="archive-title" id="{{t | downcase | replace:" ","-" }}">{{ t }}</h2>
<ul class="tag-list">
{% for post in posts %}
  {% if post.tags contains t %}
  <li>
    <a class="archive-link" href="{{ post.url }}">{{ post.title }}</a> 
    <span class="date">{{ post.date | date: "%-d %B %Y" }}</span>
  </li>
  {% endif %}
{% endfor %}
</ul>

---

{% endfor %}
