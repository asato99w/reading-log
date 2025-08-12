# Chapter 10: Supple Design

## Chapter Overview
Presents design patterns that make domain models flexible and expressive, enabling easy combination and extension of domain operations.

## Main Content

### Intention-Revealing Interfaces
- Method and class names should clearly communicate their business purpose and effects
- Interfaces should express what operations accomplish rather than how they work internally
- Side effects and preconditions should be obvious from interface design
- Client code should read naturally using ubiquitous language when calling domain operations

### Side-Effect-Free Functions
- Operations that return information without modifying state reduce complexity and enable composition
- Pure functions can be combined freely without concern for unintended interactions
- Query operations should be clearly distinguished from command operations
- Functional style enables more sophisticated domain logic through safe composition

### Assertion and Specification Patterns
- Business rules can be expressed as explicit assertion objects that can be tested and reused
- Specification objects encapsulate business criteria in composable, testable forms
- Complex business logic becomes more manageable when broken into explicit rule objects
- Specifications enable flexible querying and validation using domain language

## Key Points
- **Interface Clarity**: Well-designed interfaces communicate business intent clearly and reduce cognitive load for developers using domain objects
- **Compositional Safety**: Side-effect-free operations enable complex domain logic through safe combination of simpler operations
- **Rule Reification**: Making business rules explicit as objects enables sophisticated business logic while maintaining code clarity and testability