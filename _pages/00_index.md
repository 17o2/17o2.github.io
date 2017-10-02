---
permalink: /
layout: default
---

<article class="coolcontainer">

  <div class="cool light">
    <h2>Personal work</h2>
    <div style="text-align:left;">
    <ul>
    <li> <a href="projects/">Projects</a> </li>
    <li> <a href="designart/">Design & Art</a> </li>
    <li> <a href="academic/">Academic</a> </li>
    <li> <a href="fun/">Fun</a> </li>
    </ul>
    </div>
  </div>

  <div class="cool dark">
    <h2>Professional work</h2>
    <div style="text-align:left;">
    <ul>
    <li> <a href="freelance/">Showcase</a> </li>
    <li> <a href="references/">Rererences</a> </li>
    <li> <a href="hireme/">Hire me</a> </li>
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
