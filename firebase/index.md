---
layout: page
title: Firebase
excerpt: "From foundations to full-stack & mobile apps"
modified: 2017-01-30T15:00:00.000000-05:00
image:
  feature: firebase-mountain.png
  credit: Unsplash
  creditlink: https://unsplash.com/search/mountain?photo=x2Miv4owGEM
---


<ul class="post-list">
{% for post in site.categories.firebase %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
