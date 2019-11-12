---
layout: default
title: Articles
---
# {{page.title}}

<section>
	
   {% for post in site.posts %}
       <!-- {% assign currentDate = post.date | date: "%B %Y" %}
       {% if currentDate != myDate %}
           {% unless forloop.first %}</ul>{% endunless %}
           <h1>
					 {{ currentDate }}
					 </h1>
           <ul>
           {% assign myDate = currentDate %}
       {% endif %} -->
			 
       	<li>
			 		<a href="{{ post.url }}">
					 {{ post.title }}
					</a>
				</li>
       {% if forloop.last %}{% endif %}
   {% endfor %}

</section>
