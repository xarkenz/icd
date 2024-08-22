---
layout: home
title: Introduction to Compiler Design
---

## Welcome to ICD!

Interested in compilers? You're in the right place! See the [About]({{site.url}}/about/)
page for more information about this course.

You can sign up for the course at any time [here]({{site.url}}/signup/).

(Note that the main purpose of this sign-up form is so I can keep you updated via email
announcements. To stop receiving updates, just let me know in an email.)

## Lectures

{% if site.lectures_24f != empty %}
  <ul>
    {% for lecture in site.lectures_24f %}
      <li>
        <a href="{{site.url}}{{lecture.url}}">{{lecture.title}}</a>
      </li>
    {% endfor %}
  </ul>
{% else %}
  No lectures have been given for this semester yet!
  For a preview of the topics we'll be going over this semester, feel free to
  take a look at the lectures from [last semester]({{site.url}}/lectures_24s/).
{% endif %}

{% if site.bonus_lectures_24f != empty %}
  <h2>Bonus Lectures</h2>

  <ul>
    {% for lecture in site.bonus_lectures_24f %}
      <li>
        <a href="{{site.url}}{{lecture.url}}">{{lecture.title}}</a>
      </li>
    {% endfor %}
  </ul>
{% endif %}

## Resources

- [LLVM-IR Language Reference Manual](https://llvm.org/docs/LangRef.html)
- [ICD Example Compiler](https://github.com/xarkenz/icd-example) (written in Java)
- [ECCO Example Compiler](https://github.com/CharlesAverill/ECCO) (written in Python)

## Archive

- [Spring 2024]({{site.url}}/lectures_24s/)
  ([Sean Clarke])
- [Fall 2023](https://charlesaverill.github.io/teaching/ICD)
  ([Charles Averill])
- [Spring 2023](https://charlesaverill.github.io/teaching/PCD)
  ([Charles Averill])

[Charles Averill]: https://charlesaverill.github.io/
[Sean Clarke]: https://github.com/xarkenz/
