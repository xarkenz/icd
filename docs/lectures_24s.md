---
layout: page
title: Spring 2024 Lectures
permalink: /lectures_24s/
---

## Lectures

<ul>
  {% for lecture in site.lectures_24s %}
    <li>
      <a href="{{site.url}}{{lecture.url}}">{{lecture.title}}</a>
    </li>
  {% endfor %}
</ul>

{% if site.bonus_lectures_24s != empty %}
  ## Bonus Lectures

  <ul>
    {% for lecture in site.bonus_lectures_24s %}
      <li>
        <a href="{{site.url}}{{lecture.url}}">{{lecture.title}}</a>
      </li>
    {% endfor %}
  </ul>
{% endif %}
