---
layout: page 
title: "Posts" 
permalink: /posts/
---

These are my posts: 

{{ page.title | upcase}}

{% for post in site.posts %}
   [{{ post.title }}]({{ site.url }}{{ post.url }})    
      {{ post.excerpt }}   

{%- endfor -%}
