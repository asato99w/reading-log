# Chapter 12: Facade (Structural)

## Chapter Overview
Provides a unified interface to a set of interfaces in a subsystem, defining a higher-level interface that makes the subsystem easier to use.

## Main Content

### Intent and Structure
- Provide simple interface to complex subsystem containing many interdependent classes
- Hide complexity of subsystem from clients by wrapping it with simpler interface
- Promote weak coupling between subsystem and its clients
- Layer subsystem to provide multiple levels of abstraction

### Pattern Participants
- **Facade**: Provides convenient interface to subsystem, delegates client requests to appropriate subsystem objects
- **Subsystem Classes**: Implement subsystem functionality, handle work assigned by Facade, have no knowledge of Facade

### Implementation Considerations
- Facade doesn't prevent clients from accessing subsystem classes directly if needed
- Multiple facades can be provided for different subsystem aspects or client types
- Facade can be implemented as Singleton when only one facade instance is needed
- Abstract Facade can be used to support multiple implementations of subsystem

## Key Points
- **Simplified Interface**: Facade provides simplified interface that covers most common use cases of complex subsystem
- **Reduced Coupling**: Clients depend on Facade rather than many subsystem classes, reducing coupling and dependencies
- **Layered Design**: Supports layered architecture where each layer uses Facade to access layer below