---
title: Personal projects
shorttitle: Personal
category: personal
permalink: /personal/
hideinnavbar: true
---

<ul>
{% assign subcats = site.pages | where:"category",page.category %}
{% for eachpage in subcats %}
{% if forloop.first == false %}
<li><a href="{{ eachpage.permalink }}">{{ eachpage.title }}</a></li>
{% endif %}
{% endfor %}
</ul>
