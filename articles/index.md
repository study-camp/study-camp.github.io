---
layout: page
title: Recent Articles
excerpt: "Archive of articles sorted by date."
search_omit: true
image:
  feature: article-climb.png
  credit: Unsplash
  creditlink: https://unsplash.com/search/climb?photo=Lu2pfy_8VKg
---

<ul class="post-list">
{% for post in site.categories.articles %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
