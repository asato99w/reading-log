# Chapter 2: Degenerate Objects

## Chapter Overview
Building on the fake implementation from Chapter 1, this chapter addresses the problem of side effects by making Dollar objects immutable. Introduces the concept of value objects and demonstrates how TDD drives toward better object-oriented design.

## Main Content
- **Side Effects Problem**
  - Identifying issues with mutable Dollar objects
  - Understanding how mutation can break tests and cause confusion
  - Recognizing the need for immutable value objects
  - Learning to spot design problems through test failures

- **Value Object Implementation**
  - Making Dollar.times() return a new Dollar instead of modifying existing one
  - Understanding the value object pattern and its benefits
  - Implementing immutability to eliminate side effects
  - Creating objects that represent values rather than entities

- **Test Evolution**
  - Updating tests to work with immutable objects
  - Understanding how design changes affect existing tests
  - Learning to refactor tests alongside production code
  - Maintaining green while improving design

## Key Points
- Immutable value objects eliminate side effects and make code more predictable and testable
- TDD helps identify design problems early through test failures and awkward test code
- Small design improvements often emerge naturally from trying to make tests work cleanly