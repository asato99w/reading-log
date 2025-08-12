# Chapter 7: Apples and Oranges

## Chapter Overview
Addressing the problem of Dollar-Franc comparison by extracting a common Money superclass. Demonstrates how refactoring emerges naturally from duplication and how inheritance can be introduced incrementally while maintaining green tests.

## Main Content
- **Common Superclass Extraction**
  - Creating Money class as parent for both Dollar and Franc
  - Moving common behavior (amount field, equals method) to superclass
  - Refactoring inheritance hierarchy while maintaining all tests green
  - Understanding how to introduce inheritance incrementally

- **Consolidated Equality Implementation**
  - Moving equals() method to Money superclass
  - Ensuring Dollar and Franc objects are not equal to each other
  - Implementing class-based equality checking
  - Maintaining correct behavior while removing duplication

- **Inheritance Design Principles**
  - Using inheritance to share common behavior
  - Understanding when subclassing is appropriate
  - Maintaining substitutability (Liskov Substitution Principle)
  - Balancing code reuse with clear design

## Key Points
- Extract superclass when you have duplication between related classes that suggests common abstraction
- Move common behavior to superclass incrementally, ensuring tests stay green throughout the process
- Use class comparison in equality methods when objects of different subclasses should not be equal