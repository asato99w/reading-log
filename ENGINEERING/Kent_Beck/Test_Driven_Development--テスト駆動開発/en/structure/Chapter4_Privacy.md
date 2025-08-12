# Chapter 4: Privacy

## Chapter Overview
Making the Dollar's amount field private to enforce encapsulation and demonstrate how TDD supports good object-oriented design principles. Shows how external behavior testing enables internal implementation changes.

## Main Content
- **Encapsulation Implementation**
  - Making the amount field private in the Dollar class
  - Understanding how encapsulation protects object invariants
  - Ensuring that object behavior is accessed only through defined interfaces
  - Demonstrating that tests should focus on behavior, not implementation

- **Test Independence from Implementation**
  - Showing how well-designed tests remain valid when internal implementation changes
  - Understanding the difference between testing behavior and testing state
  - Learning to write tests that are robust to internal refactoring
  - Maintaining test validity while improving design

- **Object-Oriented Design Principles**
  - Applying encapsulation to hide implementation details
  - Understanding how TDD supports good OO design practices
  - Creating objects with clear, well-defined interfaces
  - Building objects that maintain their own integrity

## Key Points
- Good tests focus on object behavior rather than internal state or implementation details
- Encapsulation can be implemented safely when tests verify external behavior rather than internal structure
- TDD naturally drives toward better object-oriented design by emphasizing interface over implementation