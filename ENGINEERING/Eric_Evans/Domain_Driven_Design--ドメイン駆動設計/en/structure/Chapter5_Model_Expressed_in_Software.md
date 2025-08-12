# Chapter 5: A Model Expressed in Software

## Chapter Overview
Defines fundamental tactical patterns (Entity, Value Object, Service) that form the vocabulary for expressing domain concepts in object-oriented code.

## Main Content

### Entity Pattern
- Objects with distinct identity that persists through lifecycle changes
- Identity equality rather than attribute equality defines entity comparison
- Entities may change attributes while maintaining identity continuity
- Identity must be carefully designed to remain stable and meaningful throughout entity lifecycle

### Value Object Pattern
- Objects defined entirely by their attributes without distinct identity
- Immutable objects that can be freely shared and replaced without side effects
- Equality based on all attributes rather than object identity
- Value objects should be designed as complete conceptual units representing domain concepts

### Service Pattern
- Operations that don't naturally belong to any specific entity or value object
- Stateless operations that coordinate between multiple domain objects
- Services should use ubiquitous language and focus on domain operations
- Should be used sparingly to avoid creating anemic domain models with all logic in services

## Key Points
- **Identity vs. Value**: Clear distinction between entities (identity-based) and value objects (attribute-based) provides foundation for proper domain modeling
- **Immutability Benefits**: Value objects' immutability eliminates many concurrency and state management issues while simplifying reasoning about domain operations
- **Service Restraint**: Domain services should complement entity and value object behavior rather than replace it, maintaining rich domain models