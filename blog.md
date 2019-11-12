---
layout: default
title: blog
---
	
{% for post in site.posts limit:10 %}
<h1>{{post.title}}</h1>
{{ post.content }}
<h2>written on {{post.date | date: "%B %-d, %Y"}}</h2>	
{% endfor %}
