# Chapter 6: Composing Methods

## Chapter Overview
This chapter begins the refactoring catalog with techniques for organizing code within methods. These are the most frequently used refactorings, addressing the common problem of methods that are too long or complex.

## Main Content
- **Extract Method**
  - Most important and frequently used refactoring
  - Turn code fragment into method with meaningful name
  - Mechanics for handling local variables and parameters
  - Key to making code readable and reusable

- **Inline Method**
  - Replace method call with method body
  - Used when indirection doesn't add value
  - Inverse of Extract Method
  - Helpful before re-extracting differently

- **Temp Variable Refactorings**
  - Inline Temp: Replace temp with expression
  - Replace Temp with Query: Replace temp with method call
  - Introduce Explaining Variable: Name complex expressions
  - Split Temporary Variable: One temp per assignment
  - Remove Assignments to Parameters: Use local variables instead

- **Method Object Pattern**
  - Replace Method with Method Object: Complex method becomes class
  - Useful when method has many local variables
  - Enables further refactoring of complex algorithm
  - Alternative to passing many parameters

## Key Points
- Well-composed methods are short, focused, and well-named
- Temporary variables often indicate extraction opportunities
- Method extraction is the foundation for most other refactorings