---
title: Program State as Graph
author: craig
ProgrammingLanguage: Java
ProgrammingParadigm: object-oriented
ConceptualAdvantage: "Graphs make the relevant parts of program state explicit and support detailed explanations by instructor."
Form: Representation
DrawsAttentionTo: "Program state, and especially variables and references."
UseWhen: "To demonstrate how Java code advances through a computation, e.g., when working data structures."
Cost: "Quick and easy to use, even when live-coding a solution"
OriginSource: "Interview, James Riely"
image: ProgramStateAsGraph.jpg
Mapping:
  "stack frame": "red rectangle, with method name and line number in left compartment, boxes for paremeters and local variables in right compartment"
  "object": "purple rectangle, with class name in left compartment, boxes for instance variables in right compartment"
  "array": "blue rectangle consisting of boxes for elements"
  "static fields": "yellow rectangle, with class name in left compartment, boxes for class variables in right compartment"
  "variable": "box inside a rectangle"
  "reference value": "solid arrow pointing to a rectangle"
  "primitive value": "value written inside a box"
  "callee-caller relationship": "dashed red arrow from callee stack frame to caller stack frame"
Topic: "State"
---

James Riely [developed and described a tool](https://fpl.cs.depaul.edu/jriely/visualization/), in the form of a Java class, [Trace.java](https://fpl.cs.depaul.edu/jriely/visualization/Trace.java), that produces graph representations of the Java program state in the form of GraphViz dot graphs.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/B2ucxRf8Lq0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Example Usage

He uses it in his [CSC300](http://fpl.cs.depaul.edu/jriely/ds1/index.html) course at DePaul University. Here is one of the lecture videos,
showing the traversal of linked lists.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/arIFfd2v6m8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
