---
title: Grammar as Train Track
author: matthias
ProgrammingLanguage: BNF / EBNF
ProgrammingParadigm: declarative
ConceptualAdvantage: "Pushing a train engine through the track makes visible the process of interpretation (generation or parsing) of the grammar (that is the track)."
Form: Analogy
DrawsAttentionTo: "The process of parsing or generating driven by a grammar."
UseWhen: "Introducing formal grammars (BNF / EBNF)."
Cost: "Space to build train track (non-trivial grammars will need multiple large tables or significant floor space)."
OriginSource: "Own practice, based on 'railroad diagrams'"
image: GrammarAsTrainTrack.jpg
Mapping:
  "grammar rule": "a train track with a start and an end"
  "parsing or generating": "pushing a train engine through the train track"
  "terminal symbol (in a grammar rule)": "tunnel representing a terminal symbol, generating or recognizing the text with which it is labeled"
  "non-terminal symbol (in a grammar rule)": "tunnel representing a non-terminal symbol, invoking the rule mentioned on its label"
  "sequence": "track segment going from one tunnel to the next"
  "selection": "two switches to split and join the track, requiring the train engine to decide which track to take"
  "repetition": "two switches allowing the train engine to go back and repeat a part of the grammar multiple times"
Topic: "Other"
---

The idea is described under the name "Language Trains",
one of three different "programming languages" that strive to eliminate abstraction, in the following paper:

{% include paper.html
   authors="Matthias Hauswirth, Andrea Adamoli, and Mohammad Azadmanesh"
   url="https://dl.acm.org/doi/10.1145/3141880.3141894"
   title="The Program is the System"
   publication="Koli Calling '17" %}

This notional machine was used to explain grammars to high school students and the general public in the 10-year anniversary exhibition
of the Faculty of Informatics of USI.

It was further used, in a virtual form, in a [course on programming language concepts](https://informa.inf.usi.ch/course/pithn7zetALFSrLsF/themes) for high school informatics teachers in the Swiss state of Ticino:

<img src="/assets/images/nm/GrammarAsTrainTracks1.png" class="ui fluid bordered image">

<img src="/assets/images/nm/GrammarAsTrainTracks2.png" class="ui fluid bordered image">

<img src="/assets/images/nm/GrammarAsTrainTracks3.png" class="ui fluid bordered image">

### Usage Note

Non-terminal symbols appearing in a grammar rule mean that one has to take an additional train engine to start processing the rule of that non-terminal (i.e., one needs multiple train engines, and it can be confusing to understand which prior engine to go back to when one finishes the track of a rule).
