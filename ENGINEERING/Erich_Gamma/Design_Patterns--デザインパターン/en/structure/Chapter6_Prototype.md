# Chapter 6: Prototype (Creational)

## Chapter Overview
Specifies the kinds of objects to create using a prototypical instance, and creates new objects by copying this prototype.

## Main Content

### Intent and Structure
- Create objects by cloning existing prototype instances rather than constructing from scratch
- Specify object types through prototypical instances rather than classes
- Enable runtime object creation when classes are determined dynamically
- Reduce subclassing when product classes differ only in state or configuration

### Pattern Participants
- **Prototype**: Interface declaring clone operation for duplicating itself
- **ConcretePrototype**: Implements clone operation to copy itself
- **Client**: Creates new objects by asking prototype to clone itself

### Implementation Considerations
- Clone operation must handle deep vs. shallow copying appropriately
- Prototype registry can manage and provide access to different prototype instances
- Cloning may be more efficient than creating and initializing objects from scratch
- Care needed with objects containing references to other objects during cloning

## Key Points
- **Dynamic Object Creation**: Prototype enables object creation based on runtime configuration rather than compile-time class specification
- **Efficient Creation**: Cloning can be more efficient than construction when initialization is expensive
- **Configuration Preservation**: New objects inherit complex state and configuration from prototype without requiring explicit setup