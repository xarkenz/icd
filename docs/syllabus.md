---
layout: page
title: Syllabus
permalink: /syllabus/
---

## Course Information

- **Term:** Spring 2024
- **Instructor:** Sean Clarke ([sean.clarke@utdallas.edu](mailto:sean.clarke@utdallas.edu))
- **Course Website:** [xarkenz.github.io/icd](https://xarkenz.github.io/icd)
- **Class Hours:** Monday & Wednesday, 2:30 - 3:45 pm (subject to change)
- **Class Location:** *TBD*
- **Office Hours:** during class

## Course Description

This course will provide a broad introduction to compiler design, focused specifically on code generation.
This course will not provide credit for any degree from the University of Texas at Dallas or any other
university. Upon completing this course, students will be rewarded with the **University of Texas at
Dallas Certification in Compiler Design**.
By the end of this course, students will have built a functioning compiler for either a subset of C should
they choose to follow along with the course material, or their own imperative programming language should
they choose to do so.
This course will briefly cover popular compiler design technologies, such as `flex` and `bison`, but will not
use them in the material. Instead, a scanner and parser will be built from scratch. Students are given
free reign to implement functionality in their compiler as they see fit, so implementation of these popular
technologies is allowed. From-scratch implementation is encouraged, however, to ensure that students have
a better working understanding of the internals of a basic compiler.

## Soft Prerequisites (not required)

- **CS 2336 / CS 2337** or equivalent experience in an imperative programming language (C, C++, Java, Python, etc.).
The course will be primarily taught in Python, so familiarity is encouraged. However, confidence in another language
will suffice, as no specific Python features will be important.
- **CS 2340** or equivalent knowledge of basic programming in any assembly language.
- **CS 3345** or equivalent knowledge of linked lists, trees, basic hash tables, and their traversals.
- **CS 3377** or equivalent knowledge of basic Unix, Bash usage.
- Basic Git knowledge.
- Provided course materials assume compilation to a Linux target, so **usage of Linux** in some capacity
is required, unless students choose not to use the [project base](https://github.com/CharlesAverill/ECCO).
This can be a physical Linux machine, the `cs1.utdallas.edu` server, Windows Subsystem for Linux, etc.

These prerequisites are covered in more detail on the [Prerequisites]({{site.url}}/prereqs/) page.

## Course Objectives

Successful students will:

1. Design a compiler for either a subset of C or a language of their choice
2. Implement extra features as optional homework
3. Learn how common high-level structures such as loops, conditional statements, functions, and more
can be parsed into Abstract Syntax Trees and mapped to generated LLVM-IR pseudo-assembly code.
4. Learn how to apply simple optimizations to parsed high-level code and abstract syntax trees in order
to improve generated pseudo-assembly code
5. Compare the (relatively) naive approaches presented in this course to production-level approaches
found in compilers like `gcc` and `clang`
6. Complete knowledge-testing quizzes in class

## Optional Materials

- ["Compilers: Principles, Techniques, and Tools" - Alfred V. Aho, Ravi Sethi, Jeffrey D. Ullman](https://github.com/KnowNo/books-7/blob/master/Programming/Compilers%20-%20Principles%20Techniques%20and%20Tools%20by%20Alfred%20Aho%20-%20Monica%20Lam-%20Ravi%20Sethi-%20Jeffrey%20Ullman%20-%20Second%20Edition.pdf)
- [SubC](https://www.t3x.org/subc/index.html)
- [ACWJ - DoctorWkt](https://github.com/DoctorWkt/acwj)
- [LLVM’s "My First Language Frontend"](https://llvm.org/docs/tutorial/MyFirstLanguageFrontend/index.html)
- [LLVM-IR Language Reference Manual](https://llvm.org/docs/LangRef.html)

## Quizzes (TBD)

Once-weekly in-class quizzes will be given to ensure that students are keeping up with course content.
Quizzes may be of any form as the instructor sees fit, and answers will be graded for correctness with
partial credit where applicable.

## Class Project

The main goal of this course is for students to have a functioning, hand-built compiler by the end of the
course. There is no requirement for students to compile any specific language, or to write the compiler in
any specific language. A project base will be provided to offer argument parsing, documentation generation,
and automatic testing, but it is not required for students to use the project base. Completion of any 75%
of the selected topics (including required topics listed in the Calendar) is required to receive a certification.

## Calendar

The order of later topics is subject to change. After week 4, much of the higher-level constructs can be
implemented in any order. **Bold** topics are required to earn the certification.

|Week |Dates        |Content |Optional Features |Tech Talk |
|-----|-------------|--------|------------------|----------|
|1    |1/22<br>1/24 |**Scanning**<br>**Parsing**<br>**Precedence** |Bit-shifting operators | |
|2    |1/29<br>1/31 |**LLVM generation** |Your own cool statement |General-Purpose Parsing |
|3    |2/5<br>2/7   |**Basic `print` statements** |Integer types (except `char`) | Architecture of Large Compilers |
|4    |2/12<br>2/14 |**Global Variables** |N-base integer literals |Compiler Security |
|5    |2/19<br>2/21 |**Comparisons**<br>**`if` statements**<br>**`while` loops**<br>`for` loops |`break`<br>`continue` | |
|6    |2/26<br>2/28 |**Function declarations and calls**<br>`char` type |`while`-`else` loops<br>`for`-`else` loops |JIT Compiling |
|7    |3/4<br>3/6   |**Pointers** | |Functional Language Compilation |
|8    |3/11<br>3/13 |Catch-up week (Spring Break) | | |
|9    |3/18<br>3/20 |**Basic optimizations**<br>Generalizing lvalues | | |
|10   |3/25<br>3/27 |**Function arguments**<br>Local variables (part 1) | |LLVM Optimizations |
|11   |4/1<br>4/3   |Local variables (part 2) | |Loop Optimizations |
|12   |4/8<br>4/10  |**Naive arrays** | |Higher-level language constructs |
|13   |4/15<br>4/17 |**Structs** | |Parallelism Optimizations |
|14   |4/22<br>4/24 | |Triple test |Certified Compilers<br>Zero-Knowledge Proofs in Compilers |
|15   |4/29<br>5/1  |Compiler presentations | | |

## Course Policies

### During Class

I understand that the electronic recording of notes will be important for class and so computers will be
allowed in class. Please refrain from using computers for anything but activities related to the class. Eating
and drinking are allowed in class but please refrain from it affecting the course. Try not to eat your lunch
in class as the classes are typically active.

### Attendance

There is lots of material to cover, so please attend all classes in order to stay up. If you miss a class,
reviewing the related [ACWJ](https://github.com/DoctorWkt/acwj) topics is a good way to catch back up.

### Recordings

The course lectures will be recorded and uploaded to YouTube for student convenience.

## Academic Integrity and Honesty

Please don’t copy code from ACWJ if you can help it. It’s tempting because we’re following its evolution
very closely, but it’s a lot more fun and rewarding to implement everything based on what you learn in
class. The ECCO source code also implements everything we talk about in class, please don’t copy from
there either.

## UTD Syllabus Policies and Procedures

The information contained in the following link constitutes the University’s policies and procedures segment
of the course syllabus. Please go to [go.utdallas.edu/syllabus-policies](http://go.utdallas.edu/syllabus-policies) for these policies.
