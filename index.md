---
layout: index
title: Updates
date: 2020-03-06
---

<h3>2021 Local 40 Election</h3>
  <ul>
    {% for post in site.posts %}
      {% assign date_format = site.cayman.date_format | default: "%b %-d, %Y" %}
      <h4>
          <a class="post-link" href="{{ site.baseurl }}{{ post.url}}" title="{{ post.title }}">{{ post.title | escape }}</a>
      </h4>
      <span class="post-meta">{{ post.date | date: date_format }}
      </span>
      {{ post.excerpt | markdownify | truncatewords: 30 }}
    {% endfor %}
  <ul>
