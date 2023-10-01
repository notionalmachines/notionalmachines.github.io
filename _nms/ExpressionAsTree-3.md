---
title: "Expression as Tree (3 - Objects)"
sequence: "Expression as Tree"
Step: 3
StepTitle: "Objects"
author: matthias
ProgrammingLanguage: Java
ProgrammingParadigm: imperative, OO
ConceptualAdvantage: "Makes explicit the fact that object allocation, method invocation, and field access are just expressions and can be composed like any other expression."
Form: Representation
DrawsAttentionTo: "The structure, typing, and evaluation of expressions involving instances and classes."
UseWhen: "When explaining nesting and chaining of method calls and constructor calls, class vs. instance method and field accesses, null, and this."
Cost: "Small, can be done on paper or with a tool like Expression Tutor."
OriginSource: "Own practice"
image: ExpressionAsTree-3.jpg
Mapping:
  "...": "(all aspects from 2-Logic)"
  "null": "tree node containing 'null'"
  "this": "tree node containing 'this'"
  "instantiation": "tree node with 'new', class name, and a parentheses containing comma-separated holes for constructor parameters"
  "variable": "tree node containing name of variable of an Object type"
  "instance field access": "tree node containing a hole, a dot, and a field name"
  "instance method invocation": "tree node with a hole, a dot, and parentheses containing comma-separated holes for method parameters"
  "class field access": "tree node containing class name, a dot, and a field name"
  "class method invocation": "tree node with class name, a dot, and parentheses containing comma-separated holes for method parameters"
Topic: "Expressions"
---

The following videos and activities come from [ExpressionTutor.org](https://expressiontutor.org/), where you can find a much more comprehensive set of resources and tools.
Expression Tutor supports many different programming languages,
but the material discussed here is specific to Java.

The [Crash Course: Expressions in Java](https://expressiontutor.org/course/JavaExpressionsCrashCourse/part/Part%202) provides a learning experience that corresponds to this notional machine sequence.

<h4 class="ui header">Explainer Video: Expressions Involving Objects</h4>

The following video comes from section [Objects](https://expressiontutor.org/course/JavaExpressionsCrashCourse/part/Part%202/2.3) of the Crash Course.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/IF1ZVvRQQUc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<h4 class="ui header">Example expressiontutor.org Activity</h4>

Here is an example "Expression Tutor" activity. Can you solve it?

<iframe width="100%" height="904" frameborder="0" allowfullscreen src="https://expressiontutor.org/activity/do?task=615f4aea-16d1-45fe-9935-4beabcdd06d3&iframe"></iframe>

<h4 class="ui header">Explainer Video: Where to find expressions</h4>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/oDxl4K1NZ1k" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<h4 class="ui header">Explainer Video: Determining the type of an expression</h4>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/vkG2g0bMBFo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<h4 class="ui header">Explainer Video: Determining the value of an expression</h4>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/znOFVz18FuM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>