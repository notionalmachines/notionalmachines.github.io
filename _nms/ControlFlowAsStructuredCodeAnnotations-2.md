---
title: "Control Flow as Structured Code Annotations (2 - Dynamic Behavior)"
sequence: "Control Flow as Structured Code Annotations"
Step: 2
StepTitle: "Dynamic Behavior"
author: peter
ProgrammingLanguage: any
ProgrammingParadigm: imperative
ConceptualAdvantage: "The notional machine is not an entirely separate representation from the code but acts as a secondary notation to add invisible aspects of the code execution."
Form: Representation
DrawsAttentionTo: "Dynamic view of control flow (actual execution); evaluation of expressions; declaration, initialisation, access and assignment of variables."
UseWhen: "Developing understanding of how basic programming constructs work."
Cost: "Code needs carefully selected and formatted to enable annotation."
OriginSource: "Own practice, Peter Donaldson and Quintin Cutts"
image: ControlFlowAsStructuredCodeAnnotations-2.png
Mapping:
  "...": "(all aspects from 1-Static Structure)"
  "instruction execution": "add current step number to arrow leading in, then execute by adding to or looking up information in memory table, expression evaluator, or output areas"
  "expression evaluation": "copy expression, substitute values, and evaluate it in expression evaluation area"
  "variable declaration": "find first blank column in memory table and add name of variable in first row; value added underneath if initialised"
  "variable assignment": "find variable in the memory table, strike through existing entry, and add entry to row below."
  "conditionals and loops": "evaluate control expression to 'True' or 'False', then follow relevant labelled control path to next instruction"
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
