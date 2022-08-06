---
layout: page 
title: "Posts" 
permalink: /posts/
---

These are my posts: 

{% for post in site.posts %}
    {{ post.title }}
    {{ post.excerpt }}
{% endfor %}
