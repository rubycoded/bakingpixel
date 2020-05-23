---
layout: default
title: Staff
---
<h1>Staff</h1>

{% for author in site.authors %}
<h2>{{ author.name }}</h2>
<h3>{{ author.position }}</h3>
<p>{{ author.content | markdownify }}</p>
<h2>Posts</h2>
<ul>
  {% assign filtered_posts = site.posts | where: 'author', page.short_name %}
  {% for post in filtered_posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
{% endfor %}