# Chapter 29: Design Patterns

## Chapter Overview
Common design patterns that frequently emerge when practicing TDD. Understanding these patterns helps developers recognize design opportunities and implement solutions that naturally arise from test-driven development.

## Main Content
- **Command Pattern**
  - Encapsulating requests as objects to enable parameterization and queuing
  - Understanding how TDD often leads to command objects for complex operations
  - Using commands to make operations first-class citizens in the design
  - Implementing undo, logging, and queuing through command objects

- **Value Object Pattern**
  - Creating immutable objects that represent values rather than entities
  - Understanding how TDD drives toward value objects through equality testing
  - Implementing objects where equality is based on state rather than identity
  - Using value objects to eliminate aliasing bugs and improve design clarity

- **Null Object Pattern**
  - Replacing null checks with polymorphic null objects
  - Understanding how null objects simplify client code and reduce conditionals
  - Implementing meaningful behavior for "missing" or "empty" cases
  - Using null objects to eliminate special case handling

## Key Points
- TDD naturally drives toward these patterns when they solve real design problems that emerge from testing
- Recognize pattern opportunities in your code rather than forcing patterns where they don't fit
- These patterns often emerge from the need to make code more testable and remove conditionals