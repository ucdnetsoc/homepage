---
layout: page
title: Blog
permalink: /blog/
---

<div class="posts">
	<ul>
		{% for post in site.posts %}
		<li>
			<a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> -
			{{post.author}} [{{ post.date | date: "%b %d, %Y"}}]
		</li>
		{% endfor %}
	</ul>
</div>