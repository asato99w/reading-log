# Chapter 21: Counting

## Chapter Overview
Adding result collection to the testing framework to track test outcomes. Demonstrates how to build comprehensive test reporting and handle both successful and failing test cases systematically.

## Main Content
- **TestResult Implementation**
  - Creating TestResult class to collect and track test outcomes
  - Understanding how to accumulate results across multiple test executions
  - Implementing result counting for successful and failed tests
  - Building foundation for comprehensive test reporting

- **Result Collection Pattern**
  - Using collecting parameter pattern to gather results
  - Understanding how to pass result objects through test execution
  - Implementing clean separation between test execution and result reporting
  - Creating extensible result collection that can handle different outcome types

- **Test Outcome Tracking**
  - Recording test successes and failures systematically
  - Understanding how to distinguish between different types of test outcomes
  - Building data structures that support comprehensive test result analysis
  - Preparing for detailed test reporting and debugging information

## Key Points
- Separate result collection from test execution to create clean, extensible architecture
- Use collecting parameter pattern to accumulate results across multiple operations
- Build result tracking that can distinguish and count different types of test outcomes