---
layout: default
title: First Category
permalink: /firstCategory/
---

<h2>First Category</h2>

<ul class="posts">
{% for post in site.posts %}
	{% if post.categories contains "First Category" %}
		<li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
	{% endif %}
{% endfor %}
</ul>