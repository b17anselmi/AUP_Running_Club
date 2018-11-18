---
layout: page
title: Events
permalink: /events/
---
<ul>
  {% for post in site.events %}
    <li>
      <a href="{{ event.url }}">{{ event.title }}</a>
    </li>
  {% endfor %}
</ul>
