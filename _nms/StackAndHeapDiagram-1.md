---
title: "Stack and Heap Diagram (1 - Objects)"
sequence: "Stack and Heap Diagram"
Step: 1
StepTitle: "Objects"
author: matthias
ProgrammingLanguage: Java
ProgrammingParadigm: imperative, OO
ConceptualAdvantage: "Makes explicit the notion of an object, that groups together all the variables that correspond to the object's state."
Form: Representation
DrawsAttentionTo: "An object's state."
UseWhen: "Introducing the concept of an object."
Cost: "Straightforward; just draw a rounded rectangle around some variables."
OriginSource: "Own practice"
image: StackAndHeapDiagram-1.png
Mapping:
  "object": "red rounded rectangle, with class name containing instance variables"
  "instance variable": "box inside object, with name, type, value"
Topic: "Objects"
---

We use this notional machine in instruction as well as assessments
(e.g., clicker questions, mastery checks, exams).
For instruction, the instructor draws the representation.
For assessment, the student draws the representation.

The *name* of this notional machine is inspired by two of the three regions that make up the memory of the runtime environment of imperative programming languages:

* Stack: where stack frames are allocated that hold local variables and parameters of functions/procedures/methods
* Heap: where dynamically allocated memory (e.g., objects and arrays in Java) is located

The third area, "globals", could be added to the diagram, but it is less important when using an object-oriented style where static members are less prevalent.

* Globals: where global variables (e.g., static fields in Java) are located

While we primarily use this notional machine for Java, it could easily be adapted for other imperative object-oriented programming languages, such as C# or Python.

<h3 class="ui header">Notation</h3>

<h4 class="ui header">Objects, Stack Frames, and References</h4>
<img src="/assets/images/nm/StackAndHeapDiagram.png" class="ui bordered image">

<h4 class="ui header">Arrays</h4>
<img src="/assets/images/nm/StackAndHeapDiagram-Arrays.png" class="ui bordered image">

<h4 class="ui header">Origins of Notation</h4>

The *notation* for this notional machine is based on how the [BlueJ IDE](https://bluej.org/) represents objects, with a few differences:

* BlueJ only shows objects, we also show stack frames (as rectangles)
* Unlike BlueJ, we show references as arrows
* Unlike BlueJ, we refrain from associating names with objects,
to avoid the [ObjectsMustBeNamed](https://progmiscon.org/misconceptions/Java/ObjectsMustBeNamed/) misconception.
* We represent fields (and variables in general) as rectangles,
but we place the type of the variable **above** the rectangle, the name of the variable on the left, and the value inside, and we **do not show access modifiers** (private, protected, public).
* We draw a **bold** rectangle outline for `final` variables.

<img src="/assets/images/nm/StackAndHeapDiagram-BlueJ-Object.png" class="ui medium image">


<h3 class="ui header">Stack &amp; Heap Diagrams in Informa Clicker</h3>
The [Informa Clicker](http://sape.inf.usi.ch/informa) tool, a software-based classroom response system, provides a question type with an integrated editor
for stack and heap diagrams.

{% include paper.html
  authors="Matthias Hauswirth and Andrea Adamoli"
  url="https://dl.acm.org/doi/10.1145/1596655.1596657"
  title="Solve & Evaluate with Informa: A Java-based Classroom Response System for Teaching Java"
  publication="PPPJ '09" %}

<h4 class="ui header">Constructor Calls</h4>
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/Hpg4fBTCYuA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<h4 class="ui header">Local Variables</h4>
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/GXqU1QEdC58" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<h4 class="ui header">Method Calls</h4>
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/OGsd8A9tCn0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<h3 class="ui header">Web-Based Stack &amp; Heap Diagram Editor</h3>

Davide Ciulla developed a prototype of a [web based stack and heap diagram editor](https://stackandheap.netlify.app/):

<iframe src="https://stackandheap.netlify.app/" width="100%" height="600">
</iframe>
