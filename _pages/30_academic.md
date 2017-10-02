---
title: Academic work
shorttitle: Academic
category: personal
permalink: /academic/
---

{% for project in site.academic %}

## {{project.title}}
### {{ project.summary }}
{% if project.image %}
<img src="{{project.image}}" height="200" />
{% endif %}

<!-- <a href="{{ project.download }}">Download</a> -->

<article class="abstract">
{{ project.abstract }}
</article>

{% endfor %}
