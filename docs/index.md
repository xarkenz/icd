---
layout: home
title: Introduction to Compiler Design
---

## Sign Up

You can sign up for the course at any time [here]({{site.url}}/signup/).

## Lectures

<ul>
  {% for lecture in site.lectures_24s %}
    <li>
      <a href="{{site.url}}{{lecture.url}}">{{lecture.title}}</a>
    </li>
  {% endfor %}
</ul>

## Bonus Lectures

<ul>
  {% for lecture in site.bonus_lectures_24s %}
    <li>
      <a href="{{site.url}}{{lecture.url}}">{{lecture.title}}</a>
    </li>
  {% endfor %}
</ul>

## Resources

- [LLVM-IR Language Reference Manual](https://llvm.org/docs/LangRef.html)
- [ECCO Example Compiler](https://github.com/CharlesAverill/ECCO)
- [New Example Compiler](https://github.com/xarkenz/icd-example) (WIP)

## Archive

- [Fall 2023](https://charlesaverill.github.io/teaching/ICD)
  ([Charles Averill](https://charlesaverill.github.io/))
- [Spring 2023](https://charlesaverill.github.io/teaching/PCD)
  ([Charles Averill](https://charlesaverill.github.io/))