---
layout: default
title: Second Category
permalink: /secondCategory/
---

<h2>Second Category</h2>

<ul class="posts">
{% for post in site.posts %}
	{% if post.categories contains "Second Category" %}
		<li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
	{% endif %}
{% endfor %}
</ul>