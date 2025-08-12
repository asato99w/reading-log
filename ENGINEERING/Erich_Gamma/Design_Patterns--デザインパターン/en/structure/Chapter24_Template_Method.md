# Chapter 24: Template Method (Behavioral)

## Chapter Overview
Defines the skeleton of an algorithm in a base class, letting subclasses override specific steps without changing the algorithm's structure.

## Main Content

### Intent and Structure
- Define skeleton of algorithm in operation, deferring some steps to subclasses
- Let subclasses redefine certain steps without changing algorithm's structure
- Provide framework for implementing family of related algorithms
- Enable code reuse by factoring common behavior into base class

### Pattern Participants
- **AbstractClass**: Defines abstract primitive operations that concrete subclasses define to implement steps of algorithm
- **ConcreteClass**: Implements primitive operations to carry out subclass-specific steps of algorithm

### Implementation Considerations
- Template method should be final to prevent subclasses from overriding algorithm structure
- Primitive operations can be abstract (requiring implementation) or have default implementations
- Hook operations provide extension points for subclasses but have empty default implementations
- Factory methods often used as primitive operations in template methods

## Key Points
- **Algorithm Structure**: Template method defines overall algorithm structure while allowing customization of specific steps
- **Code Reuse**: Common algorithm structure implemented once in base class, reducing code duplication
- **Controlled Extension**: Subclasses can only customize specific steps, maintaining overall algorithm integrity