---
layout: default
title: Sitemap
permalink: /sitemap/
---

# Pages
{% for page in site.pages %}
2. [{% if page.title %}{{ page.title }}{% else %}{{page.url}}{% endif %}]({{ page.url }})
{% endfor %}
# Posts
{% for post in site.posts %}
2. [{{ post.title }}]({{ post.url }}) {{ post.date | date_to_string }}
{% endfor %}

