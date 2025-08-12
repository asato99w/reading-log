# Chapter 9: Times We're Livin' In

## Chapter Overview
Consolidating the times() method in the Money superclass to eliminate duplication between Dollar and Franc. Demonstrates how to move behavior to superclass while maintaining polymorphic behavior through factory methods.

## Main Content
- **Method Consolidation**
  - Moving times() method from subclasses to Money superclass
  - Eliminating duplication between Dollar and Franc implementations
  - Using factory methods to maintain correct subclass creation
  - Simplifying the inheritance hierarchy through consolidation

- **Polymorphic Factory Usage**
  - Using currency() abstract method to determine which factory method to call
  - Maintaining subclass-specific behavior through polymorphism
  - Understanding how abstract methods enable template method pattern
  - Balancing common behavior with subclass-specific requirements

- **Abstract Method Introduction**
  - Creating currency() abstract method in Money class
  - Requiring subclasses to implement currency identification
  - Using abstract methods to enforce subclass contracts
  - Understanding when abstraction is appropriate

## Key Points
- Move duplicated methods to superclass when the behavior is identical except for object creation
- Use abstract methods to capture subclass-specific behavior needed by superclass methods
- Factory methods combined with polymorphism allow superclass methods to create appropriate subclass instances