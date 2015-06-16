---
layout: page-de
title: Blog Deutsch
excerpt: "Alle Einträge im Archiv sind nach Datum sortiert."
search_omit: true
---

<ul class="post-list">
{% for post in site.categories.blog-de %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
