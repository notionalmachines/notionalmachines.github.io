---
title: Procedure as Worker
author: ben
ProgrammingLanguage: any
ProgrammingParadigm: imperative
ConceptualAdvantage: Provides a way to visualise input and action, and later the difference between action and output. The same visualisation extended to cover user defined procedures, parameters and later to explain sub-procedure calls including recursion.
Form: Analogy
DrawsAttentionTo:
UseWhen:
Cost:
OriginSource: "Own practice"
image: ProcedureAsWorker.jpg
Mapping:
  "procedure": "worker who knows how to do a particular job"
  "procedure call": "calling the name of the worker, so that he starts doing his particular job"
  "procedure input": "giving information to the worker (telling them in their right ear)"
  "procedure implementation": "instructions for the worker on how to do their job"
  "procedure effect": "how the worker affects the world"
  "procedure result": "what the worker speaks to the worker on their left"
Topic: "Functions"
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

<img src="/assets/images/nm/ProcedureAsWorker-Pipeline.png" class="ui fluid bordered image">

#### Chapter 2

Each procedure is like a **worker** who knows how to do a particular job
and will execute that job when commanded to by having his name called.

Some of these workers need information to be able to do their jobs.
Giving this information is called giving an **input**.

#### Chapter 9

We have described procedures as **workers**.
So far all the workes have been run because they produce some **effect**.
In most cases the effect has depended on an **input**.

They always listen for their input **from the right**.
The workers will only carry out their effect once they have the correct number of inputs.

There are other kinds of workers which do not produce an effect.
These workers use their inputs to calculate a **result** which they speak to the worker **on their left**.
We are unable to see this **result** unless we arrange for it to be the input of a worker who produces a visible effect.
The name of a procedure which only gives a **result** is `ADD`.
