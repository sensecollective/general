# RDF Representation in User Interfaces Team

**This is WIP!**

Clear outline of goals/motivation/mission.

## Mission statement
The general purpose of this task force will be to bridge the vastly disconnected models of RDF data structures with the user interfaces meant to encapsulate them. The implicit transformations that are commonly applied to Linked Data in order to represent them as human-readable entities are not well defined. As a consequence, developers often resort to creating their own ad hoc transformations, adding to a growing conglomerate of redundant yet non-reusable components. The lessons learned thereafter have been that creating *reusable* methods for transforming RDF structures into user interface components is not trivial since there are both many ways to interpret the structure of data, and many ways to conceptualize its representations. 

Thus the overall goal of this task force is to create a common specification for transformations (and a reference implemenation) to build graphical user interfaces based on and informed by RDF data structures.

## Goals
- Leverage the RDF data structure
- Clear separation of roles regarding definitions (@fkleedorfer: not sure what that means - would appreciate more detailed explananation)
- Enables an iterative development process
- Highly reusable outcome (the transformations can be used in other contexts)
- Handle language transparently
- Zero-input fallback
  - If there are no transformations defined a first naive rendering is provided.
  - The transformation still need to work on RDF data structures provided without an explicit ontology.
- Never show URIs
- Provide edit as well as display functionality
- Allow different GUI rendering results for the same underlying data, depending on context


## Definitions
As this is WIP, We'll clean this text up as we go along. However, right now, we have been using terms that I'm not sure we agree upon:

**Transformation** (as used in the Mission statement) is a  function: RDF Dataset -> GUI, maybe also RDF Dataset -> GUI Component, or RDF Graph -> GUI Component.

**Roles regarding definitions** (as used in Goals) is unclear: What Roles, Definition of what?

**Context** (as used in Goals): an attribute (or a more complex data structure) that characterizes a user's situation and allows for selecting one of possibly multiple transformations.

## References

### Implementations
#### phuzzy
* [paper](http://geog.ucsb.edu/~regalia/paper/voila2017.pdf)
* [website](http://phuzzy.link/)
#### uduvudu
* [paper](https://exascale.info/assets/pdf/uduvudu.pdf)
* [website](http://uduvudu.org)
#### ld-r
* [papers](http://research.ld-r.org)
* [website](http://ld-r.org/)

### papers
* [Argo](http://ceur-ws.org/Vol-135/paper8.pdf)
* [Customised Visualisations of Linked Open Data](http://ceur-ws.org/Vol-1947/paper03.pdf)

### ontologies
* [shacl](https://www.w3.org/TR/shacl/)


## Name of TF?
  - Human readeable RDF
  - Graph to Human
  - Web based User Interface Generation 
  - Layout / Templating
  - Human RDF Interaction or Human Graph Interaction
  - Semantics aware User Interfaces
  - Data aware UIs

## Direction
  - Design Pattern / Library / Ontology
  - Pipeline


## Use Cases
[Adaptive GUI for Web of Needs](usecase_won.md)
