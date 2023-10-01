---
title: Object as Student
author: matthias
ProgrammingLanguage: any
ProgrammingParadigm: object-oriented
ConceptualAdvantage: "Makes explicit that an object is an identifiable thing that answers to calls."
Form: Analogy
DrawsAttentionTo: "Objects, method calls, and returns."
UseWhen: "When the meaning of OO is still unclear."
Cost: "Difficult for instructor to react to students' actions during role-play,and to catch (and exploit) all the teachable moments."
OriginSource: "Own practice, Andrianoff & Levine"
image: ObjectAsStudent.jpg
Mapping:
  "class": "natural language description of methods and their behaviors (on sheet of paper)"
  "object": "student"
  "method call": "verbal request made to student"
  "actual argument": "stated as part of verbal request"
  "return value": "verbal response from student"
Topic: "Objects"
---

This idea is based on Andrianoff & Levine's
[Role Playing in an OO World](https://dl.acm.org/doi/10.1145/563340.563386).

Matthias Hauswirth uses this notional machine in the first week
of his object-oriented programming course.
The course follows an objects-first methodology,
and object creation and method invocation are the first concepts students learn.

This analogy-based notional machine has two main risks:

* Students may believe that objects---like students---are independent active entities
* Students may believe that method calls are asynchronous (non-blocking), i.e., that the caller continues operating while waiting for the callee's response
