---
title: Professional projects
shorttitle: Professional
category: professional
permalink: /professional/
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
