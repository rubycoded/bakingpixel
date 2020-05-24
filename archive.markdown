---
layout: page
title: Archive
permalink: /archive/
---
Here are all the posts on BakingPixel sorted by date. You can also browse posts by [tags](/tags).

{% assign postsByMonth = site.posts | group_by_exp:"post", "post.date | date: '%B %Y'" %}
{% for month in postsByMonth %}
<h2 class="archive-title" id="{{ month.name }}-{{ year.name }}">{{ month.name }} {{ year.name }}</h2>
<ul class="archive-list" aria-label="posts from {{ month.name }} {{ year.name }}">
  {% for post in month.items %}
  <li>
		<a class="archive-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a> 
    <span class="date">{{ post.date | date: "%-d %B %Y" }}</span>
  </li>
  {% endfor %}
</ul>
{% endfor %}