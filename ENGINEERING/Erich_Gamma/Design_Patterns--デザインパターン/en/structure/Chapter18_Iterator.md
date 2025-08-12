# Chapter 18: Iterator (Behavioral)

## Chapter Overview
Provides a way to access elements of an aggregate object sequentially without exposing its underlying representation.

## Main Content

### Intent and Structure
- Provide access to elements of aggregate object without exposing internal structure
- Support multiple traversals of aggregate objects simultaneously
- Provide uniform interface for traversing different aggregate structures
- Enable polymorphic iteration where same client code works with different aggregate types

### Pattern Participants
- **Iterator**: Interface for accessing and traversing elements
- **ConcreteIterator**: Implements Iterator interface, keeps track of current position in traversal
- **Aggregate**: Interface for creating Iterator object
- **ConcreteAggregate**: Implements Iterator creation to return proper ConcreteIterator instance

### Implementation Considerations
- External iterators controlled by client, internal iterators control iteration themselves
- Robust iterators remain valid when aggregate modified during iteration
- Multiple iterators can traverse same aggregate simultaneously
- Iterator can provide additional operations beyond basic traversal

## Key Points
- **Encapsulation**: Iterator provides access to elements without exposing aggregate's internal structure
- **Uniform Interface**: Same iterator interface works with different types of aggregate structures
- **Multiple Traversals**: Multiple iterators can traverse same aggregate independently and simultaneously