# Chapter 3: Equality for All

## Chapter Overview
Implementing equality for Dollar objects to enable proper testing and comparison. Demonstrates how TDD drives toward implementing fundamental object behaviors correctly and how triangulation helps ensure robust implementations.

## Main Content
- **Equality Implementation**
  - Implementing equals() method for Dollar class
  - Understanding the importance of equality for value objects
  - Starting with simple, specific implementation
  - Using triangulation to drive toward general solution

- **Triangulation Technique**
  - Writing multiple tests with different values to drive generalization
  - Understanding when you have enough examples to generalize
  - Removing duplication between test cases and implementation
  - Building confidence through multiple concrete examples

- **Value Object Behavior**
  - Establishing that objects with same value should be equal
  - Understanding the relationship between equality and immutability
  - Implementing value semantics correctly
  - Recognizing common patterns in object equality

## Key Points
- Equality is fundamental for value objects and must be implemented correctly for effective testing
- Triangulation using multiple specific examples helps drive toward robust, general implementations
- Start with simple, specific solutions and generalize only when you have multiple examples