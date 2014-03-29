---
layout: default
title: מפת אתר
permalink: /sitemap/
---
רשימה לא ממויינת של דפים ורשומות באתר. דף זה כנראה יוסר מהאתר בהמשך.

# דפים
{% for page in site.pages %}
2. [{% if page.title %}{{ page.title }}{% else %}{{page.url}}{% endif %}]({{site.baseurl}}{{ page.url }})
{% endfor %}
# רשומות
{% for post in site.posts %}
2. [{{ post.title }}]({{site.baseurl}}{{ post.url }}) {{ post.date | date_to_string }}
{% endfor %}

