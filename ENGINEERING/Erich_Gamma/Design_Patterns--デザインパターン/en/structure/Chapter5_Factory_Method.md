# Chapter 5: Factory Method (Creational)

## Chapter Overview
Defines an interface for creating objects, but lets subclasses decide which class to instantiate, deferring instantiation to subclasses.

## Main Content

### Intent and Structure
- Create objects without specifying exact classes to instantiate
- Enable subclasses to choose which class to instantiate based on context
- Promote loose coupling by eliminating need to bind application-specific classes
- Support parallel class hierarchies where creator and product hierarchies correspond

### Pattern Participants
- **Creator**: Abstract class declaring factory method returning Product object
- **ConcreteCreator**: Overrides factory method to return ConcreteProduct instance
- **Product**: Common interface for objects that factory method creates
- **ConcreteProduct**: Implements Product interface, created by ConcreteCreator

### Implementation Considerations
- Factory method can be abstract requiring subclass implementation or provide default
- Parameterized factory methods can create different product types based on arguments
- Naming conventions help identify factory methods (e.g., createProduct, makeProduct)
- Factory method often called from Template Method in creator class

## Key Points
- **Loose Coupling**: Factory Method eliminates need for client code to know about specific product classes
- **Subclass Control**: Subclasses have complete control over which product classes to instantiate
- **Parallel Hierarchies**: Supports parallel class hierarchies where creator and product classes evolve together