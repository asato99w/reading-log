# Chapter 19: Set the Table

## Chapter Overview
Adding setUp() functionality to the testing framework to initialize test fixtures. Demonstrates how common test preparation can be automated and how TDD applies to building testing infrastructure itself.

## Main Content
- **setUp() Method Implementation**
  - Adding automatic setUp() method invocation before each test
  - Understanding the fixture pattern for test preparation
  - Implementing consistent test initialization across test cases
  - Ensuring each test starts with a clean, known state

- **Test Fixture Pattern**
  - Creating WasRun.setUp() method to initialize test state
  - Understanding how fixtures eliminate test preparation duplication
  - Making test setup automatic and consistent
  - Preparing for more complex test scenarios

- **Framework Enhancement**
  - Extending TestCase to support fixture initialization
  - Using Python's dynamic method invocation for setUp()
  - Building more sophisticated test execution lifecycle
  - Adding features incrementally while maintaining existing functionality

## Key Points
- setUp() methods eliminate duplication in test preparation and ensure consistent starting conditions
- Testing frameworks can automatically invoke fixture methods to simplify test writing
- Add framework features incrementally, ensuring existing functionality continues to work