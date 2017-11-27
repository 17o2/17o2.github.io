---
title: References
permalink: /professional/references/
category: professional
---

{% for reference in site.references %}
<center>
<div style="max-width:800px">

<h2>{{ reference.name }}</h2>
<h3><a href="{{ reference.website }}" target="blank">{{ reference.company }}</a> | {{ reference.role }}</h3>
<!-- {% if reference.image %}
<img src="/academic/{{reference.image}}" height="200" />
{% endif %} -->

<!-- <a href="/academic/{{ project.download }}">Download</a> -->

<article class="abstract">
{{ reference.text }}
</article>

</div>
</center>
{% endfor %}
