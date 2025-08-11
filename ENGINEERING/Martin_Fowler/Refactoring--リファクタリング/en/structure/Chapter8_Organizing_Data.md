# Chapter 8: Organizing Data

## Chapter Overview
This chapter focuses on refactorings that improve how data is structured and accessed, making code more type-safe, intention-revealing, and flexible.

## Main Content
- **Data Access and Encapsulation**
  - Self Encapsulate Field: Use accessors even within the same class
  - Encapsulate Field: Make fields private and provide public accessors
  - Encapsulate Collection: Return read-only views and provide modification methods
  - Benefits of consistent data access patterns

- **Object-Oriented Data Structures**
  - Replace Data Value with Object: Turn primitive data into objects
  - Change Value to Reference: Make objects shareable references
  - Change Reference to Value: Make objects immutable values
  - Replace Array with Object: Use named fields instead of array indices
  - Duplicate Observed Data: Separate presentation data from domain data

- **Type Code Refactorings**
  - Replace Type Code with Class: Simple type safety improvement
  - Replace Type Code with Subclasses: Enable polymorphic behavior
  - Replace Type Code with State/Strategy: Dynamic type changes
  - Replace Subclass with Fields: Eliminate subclasses that only vary in data

- **Data Relationship Management**
  - Change Unidirectional Association to Bidirectional: Add back pointers
  - Change Bidirectional Association to Unidirectional: Reduce coupling
  - Replace Magic Number with Symbolic Constant: Named constants for literals
  - Managing object lifecycles and references

## Key Points
- Proper data organization makes code more maintainable and less error-prone
- Objects are better than primitives for representing domain concepts
- Type safety and intention-revealing code go hand in hand