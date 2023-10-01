---
title: List as Stack of Boxes
author: ben
ProgrammingLanguage: any
ProgrammingParadigm: imperative
ConceptualAdvantage: "Emphasises that only the head of list (top box) or the whole list (the stack on the pallet) is directly accessible, and that new items can be added on top of a list but not into the middle of it."
Form: Analogy
DrawsAttentionTo: "First-in, first-out property of a stack."
UseWhen:
Cost:
OriginSource: "Own practice"
image: ListAsStackOfBoxes.png
Mapping:
  "list": "stack of boxes on a pallet"
  "list element": "box on the stack"
  "[": "top of the stack"
  "]": "pallet"
Topic: "Stack"
---

This notional machine was used in the following report:

<div class="item">
  <div class="content">
    <a class="header"><a href="http://history.dcs.ed.ac.uk/archive/docs/how-to-work-the-logo-machine-dai-op-4.pdf">How to Work the LOGO Machine</a></a>
    <div class="meta">
      <span>du Boulay, J. B. H. & O'Shea, T.</span>
    </div>
    <div class="description">
      <p>DAI Occasional Paper No.4  (pp. 1-145), 1976</p>
    </div>
    <div class="extra">
      Department of Artificial Intelligence, University of Edinburgh
    </div>
  </div>
</div>

<p></p>

<img src="/assets/images/nm/ListAsStackOfBoxes-Report.png" class="ui fluid bordered image">

### Chapter 3

The beginning of a list, the top of the stack, is marked with `[` and the end of the list, the pallet is marked with `]`.
These two characters are called **list brackets**.
We call each box of the stack an **element** of the **list**.
