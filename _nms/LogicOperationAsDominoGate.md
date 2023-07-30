---
title: Logic Operation as Domino Gate
author: matthias
ProgrammingLanguage: any
ProgrammingParadigm: any
ConceptualAdvantage: "See inside logic gates/operations. Construct/invent them from atomic components, and observe/analyze their full workings."
Form: Analogy
DrawsAttentionTo: "The inner workings of a Boolean logic operation (and, or, xor)."
UseWhen: "To learn about Boolean logic operations (and, or, xor, ...)."
Cost: "Need domino pieces. Introduces an alternative real machine (e.g., implementation of domino AND is not exactly the same as implementation of electronic circuit AND). Mechanical inaccuracies can cause problems."
OriginSource: "Own practice, based on Matt Parker's 'domino computer'"
image: LogicOperationAsDominoGate.jpg
Mapping:
  "Boolean value": "domino piece (standing, or fallen)"
  "or operation": "two joining lines of dominos"
  "xor operation": "two lines of dominos like in left image"
  "and operation": "two lines of dominos like in right image"
  "function argument": "first domino piece in a line"
  "function return value": "last domino piece in a line"
Topic: "Logic"
---

The idea is described under the name "Domino Circuit",
one of three different "programming languages" that strive to eliminate abstraction, in the following paper:

{% include paper.html
   authors="Matthias Hauswirth, Andrea Adamoli, and Mohammad Azadmanesh"
   url="https://dl.acm.org/doi/10.1145/3141880.3141894"
   title="The Program is the System"
   publication="Koli Calling '17" %}

This notional machine was used to explain logic operations to high school students and the general public in the 10-year anniversary exhibition
of the Faculty of Informatics of USI.
Additionally, at the end of each exhibition day,
a four-bit full-adder built entirely from domino pieces was
used to add two numbers picked by the students:

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/EEcU0xhwvZI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The original idea of a "Domino Computer"&mdash;and [a fantastic set of related resources](http://think-maths.co.uk/downloads/domino-computer-worksheets)&mdash; comes from "stand-up mathematician" Matt Parker.
