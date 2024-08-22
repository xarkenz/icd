---
layout: page
title: Fall 2024 Lectures
permalink: /lectures_24f/
---

## Lectures

<ul>
  {% for lecture in site.lectures_24f %}
    <li>
      <a href="{{site.url}}{{lecture.url}}">{{lecture.title}}</a>
    </li>
  {% endfor %}
</ul>

{% if site.bonus_lectures_24f != empty %}
  ## Bonus Lectures

  <ul>
    {% for lecture in site.bonus_lectures_24f %}
      <li>
        <a href="{{site.url}}{{lecture.url}}">{{lecture.title}}</a>
      </li>
    {% endfor %}
  </ul>
{% endif %}
