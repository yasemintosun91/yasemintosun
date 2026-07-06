---
layout: default
title: News
permalink: /blog/
---

<h1 class="page-title">News</h1>
<p class="subtitle">Updates on publications, talks, and projects.</p>

<ul class="post-list">
  {% for post in site.posts %}
  <li>
    <div class="post-date">{{ post.date | date: '%B %-d, %Y' }}</div>
    <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>
