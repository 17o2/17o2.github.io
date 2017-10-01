---
permalink: /
layout: default
---

<article class="bubble">
<div style="display:flex;flex-wrap:wrap;align-items:center;justify-content:center;">
{% for thing in site.data.contact %}
<div style="text-align:center;padding:1em;">
<a href="{{thing.link}}"><i class='fa fa-{{thing.icon}} fa-2x'></i><br />{{thing.name}}</a>
</div>
{% endfor %}
</div>
</article>
