---
title: "Expression as Tree (1 - Arithmetic)"
sequence: "Expression as Tree"
Step: 1
StepTitle: "Arithmetic"
author: matthias
ProgrammingLanguage: Java
ProgrammingParadigm: imperative, OO
ConceptualAdvantage: "A large fraction of code consists of expressions. Students already know about expressions from school arithmetic. This notional machine makes the structure of such simple expressions explicit,
and provides a way to explain their bottom-up step-by-step evaluation."
Form: Representation
DrawsAttentionTo: "The structure of arithmetic expressions students still know from school."
UseWhen: "To reason about the structure and semantics of simple arithmetic expressions."
Cost: "Small, can be done on paper or with a tool like Expression Tutor."
OriginSource: "Own practice"
image: ExpressionAsTree-1.jpg
Mapping:
  "expression": "tree of nodes linked together"
  "operator": "node"
  "operand": "hole in a node where a child node can be attached"
  "subexpression inside expression": "subtree connected to a node's hole"
  "numerical literal": "leaf tree node labeled with the number"
  "variable": "leaf tree node labeled with name of variable of a numeric type"
  "unary + or - operator": "internal tree node with operator in front of a hole"
  "binary + - * / % operator": "internal tree node with operator between two holes"
---

The following videos and activities come from [ExpressionTutor.org](https://expressiontutor.org/), where you can find a much more comprehensive set of resources and tools.
Expression Tutor supports many different programming languages,
but the material discussed here is specific to Java.

The [Crash Course: Expressions in Java](https://expressiontutor.org/course/JavaExpressionsCrashCourse/part/Part%202) provides a learning experience that corresponds to this notional machine sequence.

<h4 class="ui header">Explainer Video: Basic Arithmetic Expressions</h4>

The following video comes from section [Arithmetic](https://expressiontutor.org/course/JavaExpressionsCrashCourse/part/Part%202/2.1) of the Crash Course.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/ac8L-GsuvgQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<h4 class="ui header">Example expressiontutor.org Activity</h4>

Here is an example "Expression Tutor" activity. Can you solve it?

<iframe width="100%" height="904" frameborder="0" allowfullscreen src="https://expressiontutor.org/activity/do?task=615f4aea-16d1-45fe-9935-4beabcdd06d3&iframe"></iframe>

<h4 class="ui header">Explainer Video: Where to find expressions</h4>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/oDxl4K1NZ1k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<h4 class="ui header">Explainer Video: Determining the type of an expression</h4>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vkG2g0bMBFo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<h4 class="ui header">Explainer Video: Determining the value of an expression</h4>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/znOFVz18FuM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>