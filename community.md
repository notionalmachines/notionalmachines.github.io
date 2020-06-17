---
title: Community
---
<h1>Community</h1>

This collection was built and is maintained by the the following collaborators.

<ul>
  {% for author in site.authors %}
    <li>
        <h2><a href="{{ author.url }}">{{ author.name }}</a></h2>
        <p>{{ author.content | markdownify }}</p>
    </li>
  {% endfor %}
</ul>