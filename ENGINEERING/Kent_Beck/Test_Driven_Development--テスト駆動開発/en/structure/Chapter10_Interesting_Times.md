# Chapter 10: Interesting Times

## Chapter Overview
Beginning the transition from simple Money objects to more complex Expression objects to handle operations like addition. Introduces the Expression interface and demonstrates how TDD guides toward more flexible, composable designs.

## Main Content
- **Expression Interface Introduction**  
  - Creating Expression interface to represent monetary operations
  - Understanding how interfaces enable flexible, composable designs
  - Preparing for complex operations beyond simple multiplication
  - Setting foundation for mathematical expression trees

- **Money as Expression**
  - Making Money implement Expression interface
  - Understanding how existing objects can be adapted to new interfaces
  - Maintaining backward compatibility while extending functionality
  - Preparing simple objects to participate in complex operations

- **Design Evolution Through Testing**
  - Using tests to drive toward more flexible architecture
  - Understanding how TDD reveals design needs organically
  - Allowing complexity to emerge when actually needed
  - Building foundations for future functionality

## Key Points
- Introduce interfaces when you need objects to participate in operations in a uniform way
- Existing classes can implement new interfaces to gain new capabilities without breaking existing functionality
- Let the need for flexibility emerge from actual requirements rather than designing it upfront