---
title: Notional Machines
---
<h1>Notional Machines</h1>

<p>
We collected the following notional machines:
</p>

<ul>
  {% for nm in site.nms %}
    <li>
        <h2><a href="{{ nm.url }}">{{ nm.title }}</a> ({{ nm.Form }})</h2>
    </li>
  {% endfor %}
</ul>
