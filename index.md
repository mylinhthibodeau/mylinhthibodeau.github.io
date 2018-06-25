---
layout: page
title: Welcome To My Personal Website
excerpt: "An archive of blog posts sorted by date."
search_omit: true
---


<div id="bg">
  <img src="images/N-of-1.png" alt="">
</div>

This website is still in its early stages. I want to launch this blog as a part of my career development endeavors !

Since I have both medical genetics clinical and bioinformatics training, I would like to share my learning journey and contribute suggestions and ideas I have to bridge the gap between clinical and bioinformatics sciences.

A lot of the material found in this blog is derived from my own personal opinion (N-of-1) and built on my journey as a trainee.  I encourage you to leave comments and share your thoughts.

Regards,

*My Linh Thibodeau*

### Recent posts

<ul class="post-list">
{% for post in site.categories.Genomics101 %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>

<ul class="post-list">
{% for post in site.categories.ClinicalBioinformatics %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>

<ul class="post-list">
{% for post in site.categories.Bioinformatics %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
