---
layout: page
title: About
permalink: /about/
---

## General Information

- **Term:** Fall 2024
- **Lecture Times:** Monday & Wednesday, 2:30 - 3:45 pm
- **Lecture Location:** TBD
- **Instructor:** Sean Clarke
  - Email: [sean.clarke@utdallas.edu](mailto:sean.clarke@utdallas.edu)
  - GitHub: [@xarkenz](https://github.com/xarkenz)

## Description

Introduction to Compiler Design is a workshop that operates in some form like a course,
though it is *not* an official course at UTD, and will not provide credit for any degree.
I am simply a student trying to help other students who are interested in designing their own compilers.
"Lectures" are given during in-person meetings, and the workshop is focused around the project
of building a compiler, which, if completed, can earn you the
**University of Texas at Dallas Certification in Compiler Design**.
(I will announce what is considered "complete" later on once I have an idea of where everyone is at.)

That said, I understand that following along and designing a compiler takes a lot of dedicated time
that not everyone has to spare, so there's no obligation to build a compiler that comes with attending.
You are welcome to come listen to the lectures and discuss compilers and programming languages
either way.

## Lecture Recordings

The course lectures will be recorded and posted on the main page of this website
alongside the lecture slides and other resources, if applicable. I will do my best to send out an
announcement once I post the recording and slides for a lecture after it occurs.

## Objectives

1. Design a compiler for either a subset of C or a similar language of your choice.
  (You may even design your own language!)
2. Learn how common high-level structures such as loops, conditional statements, functions, and more
  can be parsed into abstract syntax trees and translated into LLVM-IR pseudo-assembly code.
3. Learn how to apply simple optimizations to parsed high-level code and abstract syntax trees in order
  to improve the generated pseudo-assembly code.
4. Compare the (relatively) naive approaches presented in this course to production-level approaches
  found in compilers like GCC and Clang.

## Academic Integrity and Honesty

Please don't copy code from the example compilers or other resources if you can help it.
It's tempting because we're following the examples very closely, but it’s a lot more fun
and rewarding to implement everything on your own based on what you learned from the lectures.
I don't want to see a replica of an existing compiler, but rather an original compiler where
you apply what you have learned in a way that makes sense to you.

## Recommended Experience

- **CS 2336** or equivalent experience in an imperative programming language (C/C++, Java, Python, etc.).
- **CS 2340** or equivalent knowledge of basic programming in any assembly language.
- **CS 3345** or equivalent knowledge of linked lists, trees, basic hash tables, and their traversals.
- **CS 3377** or equivalent knowledge of basic Unix, Bash usage.
- Basic Git knowledge, along with the ability to use GitHub, Gitlab, or equivalent.
- Compilation to a Linux target is recommended in the lectures, so usage of Linux in some capacity
  will be needed if you choose to follow that advice. This can be a physical Linux machine,
  the `cs1.utdallas.edu` server, Windows Subsystem for Linux, etc.

These soft prerequisites are covered in more detail on the [Prerequisites]({{site.url}}/prereqs/) page.

## Resources

- [LLVM-IR Language Reference Manual](https://llvm.org/docs/LangRef.html)
- [ICD Example Compiler](https://github.com/xarkenz/icd-example) (written in Java)
- [ECCO Example Compiler](https://github.com/CharlesAverill/ECCO) (written in Python)

### Additional Resources and Examples

- [LLVM’s "My First Language Frontend"](https://llvm.org/docs/tutorial/MyFirstLanguageFrontend/index.html)
- [ACWJ - DoctorWkt](https://github.com/DoctorWkt/acwj)
- [SubC](https://www.t3x.org/subc/index.html)
- ["Compilers: Principles, Techniques, and Tools" - Alfred V. Aho, Ravi Sethi, Jeffrey D. Ullman](https://github.com/KnowNo/books-7/blob/master/Programming/Compilers%20-%20Principles%20Techniques%20and%20Tools%20by%20Alfred%20Aho%20-%20Monica%20Lam-%20Ravi%20Sethi-%20Jeffrey%20Ullman%20-%20Second%20Edition.pdf)
