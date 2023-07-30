---
title: "Calls as Sequence Diagram"
author: matthias
ProgrammingLanguage: any
ProgrammingParadigm: object-oriented
ConceptualAdvantage: "Make visible the flow of computation through method calls and returns, showing how calls relate to objects, and how calls and returns are paired."
Form: Representation
DrawsAttentionTo: "The idea of a method calls being communication between two objects."
UseWhen: "When introducing method calls."
Cost: "Requires the introduction of this new notation."
OriginSource: "Own practice, based on UML sequence diagrams"
image: CallsAsSequenceDiagram.jpg
Mapping:
  "method call": "solid arrow from caller activation to callee activation"
  "method return": "dashed arrow from callee activation to caller activation"
  "activation": "tall box along lifeline from call arrow to return arrow"
  "object": "box at top and lifeline down"
  "thread": "line through all calls and returns from start to finish of diagram"
Topic: "Functions"
---

This representation is inspired by [UML](https://www.omg.org/spec/UML/2.5.1/About-UML/) "Sequence Diagrams" (which describe an interaction by showing the sequence of interchanged messages).

### Description of Notation used in Course

We use this notional machine in the course "Programming Fundamentals 2"
at [USI](https://www.inf.usi.ch/en),
where we teach object-oriented programming in Java.

Assume the following classes:

```java
public class Game {
  private Pacman p = new Pacman();
  private Ghost g1 = new Ghost(p);
  private Ghost g2 = new Ghost(p);
  public void simulateStep() {
    p.step();
    g1.step();
    g2.step();
  }
}
```

```java
public class Pacman {
  public void step() {
  }
  public int distanceTo(Ghost g) {
    return ...;  // somehow compute distance between this and g
  }
  public void kill() {
    decrementLives();
    new Pill();
  }
  public void decrementLives() {
  }
}
```

```java
public class Ghost {
  private Pacman p;
  public Ghost(Pacman p) {
    this.p = p;
  }
  public void step() {
    if (p.distanceTo(this)==0) {
      p.kill();
    }
  }
}
```

```java
public class Pill {
}
```

This sequence diagram represents what could happen in a call to `Game.simulateStep()`:

<img class="ui centered image" src="/assets/images/nm/CallsAsSequenceDiagram-description.png">

#### Sequence Diagrams
A sequence diagram shows the execution of a program during a certain period of time (not necessarily starting when the program starts, but starting when a certain method gets called). In the diagram, time goes from the top to the bottom.

#### Objects and Life Lines
At the top of the diagram, draw a box for each object that already exists when the period of time represented by the diagram starts. Starting from the bottom of each box, draw a "life line" that represents the life of the object. If an object does not yet exist at the beginning, but gets created in the middle of the execution, its box appears somewhere between the top and bottom of the diagram, and its life line also starts from the bottom of its box. For any object, the life line ends at the point in time the object dies (or at the bottom of the diagram, if the object survives the duration of the diagram). In Java, we can consider that an object dies when it becomes unreachable (when there are no more references to it).

#### Method Calls and Returns
Besides the objects and their life lines, the diagram also shows method invocations and returns. Each invocation is shown with a solid arrow, from the calling object to the called object. The corresponding return is shown with a dashed arrow, from the called object back to the calling object.

An object may call a method on itself (e.g., `this.m()` or just `m()`). In this case the call and the return arrow start from the object's lifeline and end at the same object's lifeline.

#### A Note on Recursion
Note that an object calling a method on itself (e.g., `o.m()` calling `o.n()`) does **not** necessarily mean that there is a recursive method call! There only is recursion if a **method** calls itself (e.g., `o.m()` calling `o.m()`). This is different from some method of an object calling a (potentially different) method of the same object. In fact, we can have recursion also when we call the same method on a different object (`o.m()` calling `p.m()`).

### Example Usage on Whiteboard

Note that when using this notional machine in class,
we often deviate somewhat from the description above,
either to focus on a specific issue, or to save time.
In the example below, we wanted to highlight two things:

* **Calls and returns are paired**.
For every call there is a corresponding return
(later in the course, when introduce exception handling,
we will have to refine this rule).
To focus on this issue,
we use more emphasized styles for call and return arrows:
calls are solid red arrows,
and returns are dashed green arrows.
* At any point in time **only one method is actively executing**
(and that method has its stack frame on top of the call stack),
while all other activated methods are waiting for their caller to return.
Thus, at any given time, we highlight in yellow
the activation record of the executing method.

<img src="/assets/images/nm/CallsAsSequenceDiagram-full.jpg" class="ui fluid bordered image">
