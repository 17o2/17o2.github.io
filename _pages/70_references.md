---
title: References
permalink: /professional/references/
category: professional
---

{% for reference in site.references %}
<center>
<div style="max-width:800px">

<h2>{{ reference.name }}</h2>
{% if reference.image %}
<img src="/references/{{reference.image}}" height="100" />
{% endif %}
<h3><a href="{{ reference.website }}" target="blank">{{ reference.company }}</a> | {{ reference.role }}</h3>

<!-- <a href="/academic/{{ project.download }}">Download</a> -->

<article class="abstract">
{{ reference.text }}
</article>

</div>
<hr>
</center>
{% endfor %}

<!-- <center>
<h2><a href="/professional/hireme/">Hire me!</a></h2>
</center> -->
