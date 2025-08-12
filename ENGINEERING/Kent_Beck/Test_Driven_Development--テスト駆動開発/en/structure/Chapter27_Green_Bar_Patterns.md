# Chapter 27: Green Bar Patterns

## Chapter Overview
Patterns for maintaining momentum and making steady progress once you have failing tests. These patterns help developers stay productive and avoid getting stuck while working toward solutions.

## Main Content
- **Child Test Pattern**
  - Breaking down complex tests into smaller, more manageable pieces
  - Creating simpler tests when the current test seems too difficult
  - Understanding how to maintain progress by reducing scope temporarily
  - Building toward complex functionality through simpler stepping stones

- **Mock Object Pattern**
  - Using fake objects to isolate the code under test
  - Creating simple implementations that support testing without external dependencies
  - Understanding when and how to use mocks effectively
  - Building confidence through isolated testing

- **Self Shunt Pattern**
  - Having the test case object itself play the role of mock objects
  - Simplifying test setup by reducing the number of objects involved
  - Understanding when the test object can serve multiple roles
  - Balancing simplicity with clarity in test design

## Key Points
- Break down tests that seem too difficult into smaller, more achievable steps
- Use mock objects to isolate code under test and eliminate external dependencies
- The test object itself can sometimes serve as a mock, simplifying the test setup