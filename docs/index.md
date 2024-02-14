---
layout: home
title: Introduction to Compiler Design
---

## Sign Up

You can sign up for the course at any time [here]({{site.url}}/signup/).

## Lectures

<ul>
  {% for lecture in site.lectures_24s %}
    <li>[{{lecture.title}}]({{site.url}}{{lecture.url}})</li>
  {% endfor %}
</ul>

## Links

- [LLVM-IR Language Reference Manual](https://llvm.org/docs/LangRef.html)
- [ECCO Project Base](https://github.com/CharlesAverill/ECCO)
- [Fall 2023 Page](https://seashell.charles.systems/teaching/ICD)