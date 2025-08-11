# Chapter 10: Making Method Calls Simpler

## Chapter Overview
This chapter focuses on refactorings that improve method interfaces and calling conventions, making APIs clearer, simpler, and more intuitive to use.

## Main Content
- **Method Signature Refactorings**
  - Rename Method: Change method name to better reveal its purpose
  - Add Parameter: Add a parameter for information needed by method
  - Remove Parameter: Remove parameter that is no longer needed
  - Separate Query from Modifier: Divide method that returns value and changes state
  - Parameterize Method: Replace several similar methods with one parameterized method

- **Parameter and Interface Improvements**
  - Replace Parameter with Explicit Methods: Replace parameter with separate methods
  - Preserve Whole Object: Pass entire object instead of several values from it
  - Replace Parameter with Method: Receiver can obtain value by calling method
  - Introduce Parameter Object: Group parameters that naturally go together
  - Remove Setting Method: Remove setter for field that should not be changed after creation

- **Method Access and Visibility**
  - Hide Method: Make method private when it's not needed by other classes
  - Replace Constructor with Factory Method: Use factory method when constructor isn't expressive enough
  - Replace Error Code with Exception: Use exceptions instead of special error codes
  - Replace Exception with Test: Test for condition instead of catching exception

- **Interface Design Principles**
  - Clear intention through naming
  - Minimal parameter lists
  - Consistent patterns across related methods
  - Appropriate level of abstraction

## Key Points
- Good interfaces are intuitive and require minimal documentation
- Method names should clearly communicate purpose and behavior
- Parameter lists should be as short as possible while remaining clear