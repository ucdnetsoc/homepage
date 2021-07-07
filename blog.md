---
layout: page
title: Blog
permalink: /blog/
---

<div class="posts">
	<ul>
		{% for post in site.posts %}
		[{{ post.date | date: "%b %d, %Y"}}]
		<li>
			<a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> -
			{{post.author}} 
		</li>
		{% endfor %}
	</ul>
</div>