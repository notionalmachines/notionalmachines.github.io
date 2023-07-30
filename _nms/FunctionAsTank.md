---
title: Function as Tank
author: matthias
ProgrammingLanguage: any
ProgrammingParadigm: imperative or functional
ConceptualAdvantage: "Makes explicit that functions have inputs (parameters) and outputs (return value)."
Form: Analogy
DrawsAttentionTo: "Parameter passing and return value."
UseWhen: "First introducing functions."
Cost:
OriginSource: "Book, Brian Harvey"
image: FunctionAsTank.png
Mapping:
  "function": "tank"
  "parameters": "hoppers on top of tank"
  "return value": "output pipe on bottom of tank"
Topic: "Functions"
---

Brian Harvey also calls this notional machine "Plumbing Diagram".
He uses it in his book,
[Computer Science Logo Style: Symbolic Computing](https://mitpress.mit.edu/books/computer-science-logo-style-second-edition-volume-1)
(Chapter 2, Procedures, [PDF](https://people.eecs.berkeley.edu/~bh/pdf/v1ch02.pdf)).

The following example shows LOGO code and the corresponding plumbing diagram:

```logo
print word sum 2 4 "es
```

<img src="/assets/images/nm/FunctionAsTank.png" class="ui bordered image">

The book introduces the diagram as follows:

> Using the output from one procedure as an input to another procedure
> is called composition of functions.
> Some people find it helpful to look at a pictorial form of this analysis.
> We can represent each procedure as a kind of tank,
> with input hoppers on top and perhaps an output pipe at the bottom.
> (This organization makes sense because gravity will pull the information downward.)
> ...
> We can put these parts together to form a kind of “plumbing diagram” of the instruction.
> ...
> In that diagram the output pipes from one procedure
> are connected to the input hoppers of another.
> Every pipe must be connected to something.
> The inputs that are explicitly given as numbers in the instruction
> are shown with arrows pointing into the hoppers.
>
> You can annotate the diagram by indicating the actual information that flows through each pipe.
