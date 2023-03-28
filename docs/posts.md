---
layout: page 
title: "Posts" 
permalink: /posts/
---

These are my posts: 

[//]<> (Loop through pages and show the title and the first line of the page)

{% assign sorted_pages = (site.pages | where_exp: "item", "item.title != nil" | sort: 'title') %}
{% for page in sorted_pages %}
   [{{ page.title }}]({{ site.url }}{{ page.url }})    
      {{ page.excerpt }}   
{%- endfor -%}

<!-- [//]<> (Loop through posts and show the title and the first line of the post)

{{ page.title | upcase}}

{% for post in site.posts %}
   [{{ post.title }}]({{ site.url }}{{ post.url }})    
      {{ post.excerpt }}   

{%- endfor -%} -->
