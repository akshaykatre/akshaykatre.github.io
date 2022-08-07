---
layout: page 
title: "Posts" 
permalink: /posts/
---

These are my posts: 

{{ page.title | upcase}}

{% for post in site.posts %}
   {{ post.title }}  
    {{ post.excerpt }}   
   [Read more.. ]({{ site.url }}{{ post.url }})  
{%- endfor -%}
