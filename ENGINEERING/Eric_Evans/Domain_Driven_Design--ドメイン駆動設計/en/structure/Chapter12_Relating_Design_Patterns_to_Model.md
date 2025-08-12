# Chapter 12: Relating Design Patterns to the Model

## Chapter Overview
Explores integration of technical design patterns with domain modeling, ensuring patterns serve domain expression rather than obscuring it.

## Main Content

### Strategy Pattern in Domain Context
- Business rules and policies can be modeled as strategy objects that encapsulate domain behavior
- Strategy selection should be based on domain criteria rather than technical considerations
- Multiple strategies enable modeling of complex business variations and regional differences
- Strategy interfaces should use domain language and reflect business concepts

### Composite Pattern for Domain Hierarchies
- Natural business hierarchies can be effectively modeled using composite pattern
- Composite operations should reflect meaningful business operations on hierarchical structures
- Domain-specific composite behaviors enhance model expressiveness
- Hierarchical domain concepts become more manageable when properly composed

### Technical Pattern Subordination
- Design patterns must serve domain expression rather than drive model design
- Pattern application should make domain concepts clearer, not more abstract
- Technical elegance should never come at expense of domain clarity
- Patterns work best when they align naturally with business concepts and relationships

## Key Points
- **Domain-Driven Application**: Technical patterns achieve maximum value when applied to solve domain problems rather than purely technical ones
- **Expression Enhancement**: Patterns should make domain models more expressive and understandable to business stakeholders
- **Business Alignment**: Most effective pattern applications directly reflect business concepts and relationships rather than imposing technical abstractions