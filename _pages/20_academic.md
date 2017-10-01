---
title: Academic Projects
permalink: /academic/
---

{% for project in site.academic %}

## {{project.title}}
{% if project.image %}
<img src="{{project.image}}" height="200" />
{% endif %}
### {{ project.summary }}

<!-- <a href="{{ project.download }}">Download</a> -->

<article class="abstract">
{{ project.abstract }}
</article>

{% endfor %}
