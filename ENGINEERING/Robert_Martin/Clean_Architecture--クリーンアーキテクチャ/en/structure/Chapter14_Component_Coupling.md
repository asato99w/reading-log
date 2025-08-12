# Chapter 14: Component Coupling

## Chapter Overview
This chapter examines the ADP, SDP, and SAP principles for managing dependencies between components, preventing architectural degradation over time through disciplined coupling management.

## Main Content

### The Acyclic Dependencies Principle (ADP)
- Allow no cycles in the component dependency graph to prevent development and release problems
- Cyclic dependencies create situations where components cannot be independently developed or released
- Breaking cycles can be achieved through dependency inversion or creating new components
- Build systems become simpler and more reliable when component dependencies are acyclic

### The Stable Dependencies Principle (SDP)
- Depend in the direction of stability - components should depend only on components that are more stable
- Stable components are hard to change due to many incoming dependencies
- Unstable components are easy to change because few other components depend on them
- The I-metric (instability) measures the ratio of outgoing to total dependencies

### The Stable Abstractions Principle (SAP)
- A component should be as abstract as it is stable - stable components should consist of abstract classes and interfaces
- Abstract components are stable because they are hard to change but open for extension
- Concrete components should be unstable because they contain implementation details that need to change
- The A-metric (abstractness) measures the ratio of abstract classes to total classes in a component

## Key Points
1. **Dependency Management**: Proper component coupling prevents architectural degradation through disciplined dependency relationships
2. **Stability Through Abstraction**: The most stable components should be the most abstract to enable extension without modification
3. **Measurable Architecture**: Component coupling metrics provide objective measures of architectural health and design quality