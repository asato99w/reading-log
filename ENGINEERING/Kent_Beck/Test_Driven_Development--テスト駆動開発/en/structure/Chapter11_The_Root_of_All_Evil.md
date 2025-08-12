# Chapter 11: The Root of All Evil

## Chapter Overview
Implementing addition for Money objects by creating a Sum class that represents the operation. Demonstrates how TDD drives toward object-oriented solutions where operations become first-class objects rather than simple method calls.

## Main Content
- **Addition Implementation**
  - Creating Sum class to represent addition operation between Money objects
  - Understanding how operations can be modeled as objects
  - Implementing Expression interface in Sum class
  - Building composite pattern for mathematical expressions

- **Composite Pattern Application**
  - Creating expression trees where operations contain other expressions
  - Understanding how Sum can contain Money objects or other Sums
  - Building recursive evaluation through the Expression interface
  - Enabling complex expression composition

- **Bank Introduction**
  - Creating Bank class to handle expression evaluation
  - Separating expression representation from evaluation logic
  - Preparing for exchange rate handling in future chapters
  - Understanding single responsibility principle in expression evaluation

## Key Points
- Model operations as objects when they need to be manipulated, stored, or evaluated later
- Composite pattern enables building complex expressions from simple components
- Separate representation (Expression) from evaluation (Bank) to maintain single responsibility