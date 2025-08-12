# Chapter 9: Bridge (Structural)

## Chapter Overview
Separates abstraction from its implementation so that both can vary independently, avoiding permanent binding between abstraction and implementation.

## Main Content

### Intent and Structure
- Decouple abstraction from implementation to enable independent variation
- Avoid permanent binding between abstraction and implementation at compile time
- Share implementation among multiple objects while hiding implementation details from clients
- Enable platform-independent abstractions with platform-specific implementations

### Pattern Participants
- **Abstraction**: Defines abstraction interface and maintains reference to Implementor
- **RefinedAbstraction**: Extends interface defined by Abstraction with additional operations
- **Implementor**: Interface for implementation classes, doesn't need to match Abstraction interface
- **ConcreteImplementor**: Contains concrete implementation of Implementor interface

### Implementation Considerations
- Implementor interface should be minimal to maximize implementation flexibility
- Abstraction can delegate operations to Implementor or perform additional processing
- Client should work with Abstraction interface to remain independent of implementation
- Bridge can be established at runtime by configuring Abstraction with ConcreteImplementor

### Design Benefits
- Implementation changes don't require recompilation of abstraction or client code
- Abstraction and implementation class hierarchies can be extended independently
- Implementation details completely hidden from clients working with abstraction

## Key Points
- **Independent Variation**: Bridge enables abstraction and implementation to vary independently without affecting each other
- **Runtime Configuration**: Implementation can be configured at runtime, providing flexibility in object behavior
- **Implementation Hiding**: Clients work only with abstraction interface, remaining completely independent of implementation details