# Chapter 1: Refactoring, a First Example

## Chapter Overview
This opening chapter demonstrates refactoring through a complete, realistic example of improving a video rental store program. By showing rather than telling, Fowler establishes the rhythm and discipline of refactoring before introducing theory.

## Main Content
- **The Starting Program**
  - Statement generation for video rental customers
  - Monolithic method mixing calculation, classification, and formatting
  - Switch statements determining rental costs and frequent renter points
  - Difficult to modify for new requirements like HTML output

- **The Refactoring Process**
  - Decomposing the statement method into smaller pieces
  - Extracting amount calculation and frequent renter point calculation
  - Moving methods to appropriate classes (from Customer to Rental to Movie)
  - Replacing type code with polymorphism using State pattern
  - Creating separate methods for different output formats

- **Key Refactorings Applied**
  - Extract Method: Breaking down large methods
  - Move Method: Relocating behavior to appropriate classes
  - Replace Temp with Query: Eliminating temporary variables
  - Replace Type Code with State/Strategy: Using polymorphism for type-specific behavior
  - Form Template Method: Creating abstract structure for similar algorithms

## Key Points
- Small, tested steps make large transformations safe and manageable
- Refactoring makes adding new features easier by improving code structure first
- The rhythm of refactoring: test, small change, test, commit