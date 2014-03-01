---
layout: default
title: עמוד ראשי
permalink: /
---
#ברוכים הבאים. 

זהו העמוד הראשי של האתר. פה יהיה תוכן.

[מה דעתכם?]

[מה דעתכם?]: {{site.repo-url}}/../../issues/

## הודעות אחרונות בפורום
{% for item in site.data.forum %} 
* {{item.day}}-{{item.month}}-{{item.year}} [ {{item.subject}} ]( {{item.link}} )
{% endfor %}
