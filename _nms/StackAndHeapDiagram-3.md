---
title: "Stack and Heap Diagram (3 - References)"
sequence: "Stack and Heap Diagram"
Step: 3
StepTitle: "References"
author: matthias
ProgrammingLanguage: Java
ProgrammingParadigm: imperative, OO
ConceptualAdvantage: "Makes explicit the notion of a reference, which refers to a specific object, and the notion of a null value as a reference that does not point anywhere."
Form: Representation
DrawsAttentionTo: "References."
UseWhen: "Introducing the concept of references (pointers), and aliasing (multiple references pointing to the same object)."
Cost: "Straightforward; just draw an arrow."
OriginSource: "Own practice"
image: StackAndHeapDiagram-2.png
Mapping:
  "...": "(all aspects of Stack and Heap Diagram 1 - Objects)"
  "...": "(all aspects of Stack and Heap Diagram 2 - Stack Frames)"
  "reference value": "arrow from a variable rectangle (anywhere, i.e., in the stack or the heap) to an object rounded rectangle"
  "null value": "a ground symbol (i.e., the absence of an arrow)"
---

The *name* of this notional machine is inspired by two of the three regions that make up the memory of the runtime environment of imperative programming languages:

* Stack: where stack frames are allocated that hold local variables and parameters of functions/procedures/methods
* Heap: where dynamically allocated memory (e.g., objects and arrays in Java) is located

The third area, "globals", could be added to the diagram, but it is less important when using an object-oriented style where static members are less prevalent.

* Globals: where global variables (e.g., static fields in Java) are located

The *notation* for this notional machine is based on how the BlueJ IDE represents objects, with a few differences:

* Unlike BlueJ, we refrain from associating names with objects,
to avoid the [ObjectsMustBeNamed](https://progmiscon.org/misconceptions/Java/ObjectsMustBeNamed/) misconception.
* We represent fields (and variables in general) as rectangles,
but we place the type of the variable **above** the rectangle, the name of the variable on the left, and the value inside, and we **do not show access modifiers** (private, protected, public).
* We draw a **bold** rectangle outline for `final` variables.

<img src="/assets/images/nm/StackAndHeapDiagram-BlueJ-Object.png" class="ui medium image">

We use this notional machine in instruction as well as assessments
(e.g., clicker questions, mastery checks, exams).
For instruction, the instructor draws the representation.
For assessment, the student draws the representation.

<h3 class="ui header">Stack &amp; Heap Diagrams in Informa Clicker</h3>
The [Informa Clicker](http://sape.inf.usi.ch/informa) tool, a software-based classroom response system, provides a question type with an integrated editor
for stack and heap diagrams.

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
