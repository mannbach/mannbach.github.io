---
layout: default
title: "Jan Bachmann"
---
## Posts
{% for post in site.posts %}
#### {{ post.date | date: "%Y-%m-%d" }} [{{ post.title }}]({{ post.url }})
{{ post.excerpt }}
{% endfor %}
