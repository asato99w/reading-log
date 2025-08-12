# Chapter 26: Testing Patterns

## Chapter Overview
Patterns for making failing tests pass efficiently and effectively. These patterns guide developers in choosing appropriate strategies for implementing functionality once they have a failing test, emphasizing speed to green while maintaining code quality.

## Main Content
- **Fake It ('Til You Make It) Pattern**
  - Implementing the simplest possible solution to make tests pass
  - Using hardcoded values and constants as stepping stones
  - Building confidence through quick green bars before generalizing
  - Understanding when fake implementation is appropriate and valuable

- **Obvious Implementation Pattern**
  - Writing the real implementation directly when the solution is clear
  - Skipping fake implementation for simple, straightforward cases
  - Balancing speed with correctness in implementation decisions
  - Recognizing when the obvious solution is truly obvious

- **Triangulate Pattern**
  - Using multiple test cases to drive toward general solutions
  - Removing duplication systematically through generalization
  - Understanding when you have enough examples to generalize safely
  - Building robust implementations through multiple concrete examples

## Key Points
- Choose the appropriate pattern based on your confidence level and the complexity of the problem
- Fake implementation builds momentum and confidence, even when it seems "wrong" initially
- Triangulation provides safety when you're unsure about the general solution by using concrete examples to guide abstraction