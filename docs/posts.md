---
layout: page 
title: "Posts" 
permalink: /posts/
---

These are my posts: 


{% assign sorted_pages = (site.posts | where_exp: "item", "item.title != nil" | sort: 'title') %}
{% for page in sorted_pages %}   
   [{{ page.title }}]({{ site.url }}{{ page.url }})     
      {{ page.excerpt }}   
{%- endfor -%}


