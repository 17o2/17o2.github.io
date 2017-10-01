---
title: Personal Projects
permalink: /projects/
---

{% for project in site.projects %}

<h2>{{project.title}}</h2>
{% if project.image %}
<img src="{{project.image}}" height="200" class="project-image" />
{% endif %}
{{ project.summary }}
{% if project.description and false %}
<p>{{project.description}}</p>
{% endif %}
{% if project.github %}<a href="{{project.github}}">GitHub</a>{% endif %}
{% if project.hackaday %}<a href="{{project.hackaday}}">Hackaday.io</a>{% endif %}
{% if project.youtube %}<a href="{{project.youtube}}">YouTube</a>{% endif %}
{% endfor %}
