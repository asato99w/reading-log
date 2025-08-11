# Chapter 7: Moving Features Between Objects

## Chapter Overview
This chapter addresses the fundamental object-oriented design question: where should responsibilities live? It provides refactorings for redistributing behavior and data among classes.

## Main Content
- **Responsibility Distribution Refactorings**
  - Move Method: Relocate methods to more appropriate classes
  - Move Field: Relocate fields to classes that use them most
  - Extract Class: Split classes doing too much work
  - Inline Class: Merge classes that aren't pulling their weight
  - Hide Delegate: Encapsulate delegation relationships
  - Remove Middle Man: Eliminate unnecessary delegation layers

- **Extending Class Capabilities**
  - Introduce Foreign Method: Add methods to classes you can't modify
  - Introduce Local Extension: Create wrapper or subclass for external classes
  - Strategies for working with third-party libraries
  - Maintaining clean interfaces while adding functionality

- **Design Principles Applied**
  - Single Responsibility Principle in practice
  - Balancing cohesion and coupling
  - Information hiding and encapsulation
  - Law of Demeter considerations

- **Common Patterns and Solutions**
  - Feature Envy: Methods more interested in other classes
  - Data Clumps: Groups of data that belong together
  - Message Chains: Long sequences of method calls
  - Middle Man: Classes that only delegate to others

## Key Points
- Good object design places responsibilities where they belong
- Classes should have clear, focused purposes
- Delegation can be both helpful and harmful - balance is key