# Chapter 11: Decorator (Structural)

## Chapter Overview
Attaches additional responsibilities to an object dynamically, providing a flexible alternative to subclassing for extending functionality.

## Main Content

### Intent and Structure
- Add new functionality to objects dynamically without altering their structure
- Provide flexible alternative to inheritance for extending object behavior
- Enable combination of multiple extensions through decoration chaining
- Maintain interface consistency while adding responsibilities transparently

### Pattern Participants
- **Component**: Common interface for objects that can have responsibilities added dynamically
- **ConcreteComponent**: Object to which additional responsibilities can be attached
- **Decorator**: Maintains reference to Component object and conforms to Component interface
- **ConcreteDecorator**: Adds responsibilities to the component by extending Decorator behavior

### Implementation Considerations
- Decorator interface must match Component interface exactly to ensure transparency
- Decorator objects should be interchangeable and combinable in various orders
- Identity comparison may not work correctly with decorated objects
- Large numbers of small decorator classes can complicate system understanding

### Behavior and Consequences
- Decorators can be applied recursively, allowing multiple layers of functionality
- More flexible than inheritance since behaviors can be mixed and matched at runtime
- Avoids feature-heavy classes high up in hierarchy by using composition instead
- Can result in many small objects that are hard to distinguish and debug

## Key Points
- **Dynamic Extension**: Decorator allows behavior to be extended at runtime without modifying existing code or using inheritance
- **Transparent Interface**: Decorated objects maintain same interface as original, enabling seamless substitution in client code
- **Flexible Composition**: Multiple decorators can be combined in various orders to achieve different behavior combinations