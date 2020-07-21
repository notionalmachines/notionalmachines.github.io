---
title: TRACS Structured Code Annotation
author: peter
ProgrammingLanguage: any
ProgrammingParadigm: imperative
ConceptualAdvantage: makes some of the hidden execution mechanisms visible and gives a full history of the trace
Form: Representation (hand-made)
DrawsAttentionTo: ""
UseWhen: When introducing how basic programming constructs work
Cost: Example code needs to be carefully selected and formatted to avoid creating an overly difficult or time consuming annotation
OriginSource: "Personal practice developed with Quintin Cutts as part of the PLAN C project"
image: #
Mapping:
   "Control flow": Stage 1 annotate directional arrows between all possible control paths in the code
   Expressions: "Stage 1 add red rectangular outline around expressions. Stage 2 copy expression, substitute values and evaluate in expression evaluation area
   Instruction: Add current step number next to arrow leading into the instruction and then execute by updating the relevant memory table, expression evaluation and output areas
   "Variable Declaration": Find first blank column in memory table and add variable name in first row. Value added underneath if also initialised.
   "Variable Assignment": Find variable in the memory table, strike through existing entry and add entry to row below it.
   "Conditionals and Loops": "Stage 1 add a T to the control path that is followed when the expression is True and F to the other path. Stage 2 Evaluate control expression to True or False then follow relevant labelled control path to next instruction"
---
