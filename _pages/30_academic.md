---
title: Academic Work
shorttitle: Academic
category: personal
permalink: /personal/academic/
---

<!-- <div style="align-items: center;justify-content: center;width:100%"> -->
{% for project in site.academic %}
<center>
<div style="max-width:800px">

<h2>{{project.title}}</h2>
<h3>{{ project.summary }}</h3>
{% if project.image %}
<img src="/academic/{{project.image}}" height="200" />
{% endif %}

<!-- <a href="/academic/{{ project.download }}">Download</a> -->

<article class="abstract">
{{ project.abstract }}
</article>

</div>
</center>
{% endfor %}
<!-- </div> -->
