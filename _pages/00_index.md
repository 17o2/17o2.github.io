---
permalink: /
layout: default
---

<article class="coolcontainer">

  <div class="cool light">
    <a href="/personal"><h2>Personal work</h2></a>
    <div style="text-align:left;">
    <ul>
    {% assign subcats = site.pages | where:"category","personal" %}
    {% for eachpage in subcats %}
    {% if forloop.first == false %}
    <li><a href="{{ eachpage.permalink }}">{{ eachpage.title }}</a></li>
    {% endif %}
    {% endfor %}
    </ul>
    </div>
  </div>

  <div class="cool dark">
    <a href="/professional"><h2>Professional work</h2></a>
    <div style="text-align:left;">
    <ul>
    {% assign subcats = site.pages | where:"category","professional" %}
    {% for eachpage in subcats %}
    {% if forloop.first == false %}
    <li><a href="{{ eachpage.permalink }}">{{ eachpage.title }}</a></li>
    {% endif %}
    {% endfor %}
    </ul>
    </div>
  </div>

</article>

<article class="bubble">
<div style="display:flex;flex-wrap:wrap;align-items:center;justify-content:center;">
{% for thing in site.data.contact %}
<div style="text-align:center;padding:1em;min-width:15%">
<a href="{{thing.link}}" target="_blank"><i class='fa fa-{{thing.icon}} fa-2x'></i><br />{{thing.name}}</a>
</div>
{% endfor %}
</div>
</article>

<article class="bubble">
<center>
<img src="/projectimages/bc_hires.png" style="width:400px;max-width:100%">
</center>
</article>
