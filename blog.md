---
layout: default
title: Blog
---

# ✨ Cozy Blog

A warm collection of seasonal reading rituals, book club hosting ideas,  
and cozy inspiration for your home and gatherings.

<hr>

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt | strip_html | truncate: 180 }}

[Read more →]({{ post.url }})

<hr>
{% endfor %}
