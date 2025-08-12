# Chapter 5: Franc-ly Speaking

## Chapter Overview
Introducing a second currency (Franc) by duplicating the Dollar implementation. Demonstrates how TDD allows rapid progress through duplication first, with the understanding that duplication will be removed later through refactoring.

## Main Content
- **Duplication as Stepping Stone**
  - Creating Franc class by copying and modifying Dollar code
  - Understanding that duplication can be a temporary, tactical choice
  - Using duplication to quickly establish new functionality
  - Planning to remove duplication once both implementations are working

- **Rapid Progress Through Copying**
  - Getting to green quickly by reusing existing, working patterns
  - Establishing the same behavior for Franc as for Dollar
  - Building confidence through familiar, proven implementations
  - Setting up the foundation for later abstraction

- **Setting Up for Abstraction**
  - Recognizing the duplication between Dollar and Franc classes
  - Understanding that similar code suggests need for common abstraction
  - Preparing to extract common behavior into shared parent class
  - Using working examples as basis for generalization

## Key Points
- Duplication is acceptable as a temporary measure to make rapid progress toward working code
- Copy and modify can be faster than trying to generalize prematurely when you don't yet understand the full pattern
- Once you have multiple working examples, the path to abstraction often becomes clear