---
title: "Control Flow as Structured Code Annotations (1 - Static Structure)"
sequence: "Control Flow as Structured Code Annotations"
Step: 1
StepTitle: "Static Structure"
author: peter
ProgrammingLanguage: any
ProgrammingParadigm: imperative
ConceptualAdvantage: "The notional machine is not an entirely separate representation from the code but acts as a secondary notation to add invisible aspects of the code execution."
Form: Representation
DrawsAttentionTo: "Static view of control flow (possible paths), identification of expressions."
UseWhen: "Developing understanding of how basic programming constructs work."
Cost: "Code needs carefully selected and formatted to enable annotation."
OriginSource: "Own practice, Peter Donaldson and Quintin Cutts"
image: ControlFlowAsStructuredCodeAnnotations-1.png
Mapping:
  "control flow": "arrows, superimposed on the code"
  "expression": "rectangular outline around expression, superimposed on the code"
Topic: "ControlFlow"
---

Created by Peter Donaldson and Quintin Cutts /
[PLAN C project](https://trace.dcs.gla.ac.uk/planc/).

{% include paper.html
   authors="Peter Donaldson and Quintin Cutts"
   url="https://dl.acm.org/doi/10.1145/3265757.3265776"
   title="Flexible Low-cost Activities to Develop Novice Code Comprehension Skills in Schools"
   publication="WiPSCE '19" %}

### Two stages to TRACS trace

First, mark code with control flow paths and parts of the code containing expressions. Second, start at the top of the program and execute each line adding or looking up any necessary information from the memory table, expression evaluation or output areas.

<img src="/assets/images/nm/ControlFlowAsStructuredCodeAnnotations-full.png" class="ui fluid bordered image">
