# Chapter 25: Visitor (Behavioral)

## Chapter Overview
Defines a new operation without changing the classes of the objects on which it operates by creating a separate visitor hierarchy.

## Main Content

### Intent and Structure
- Define new operation without changing classes of elements on which it operates
- Separate algorithm from object structure by creating visitor hierarchy
- Enable adding new operations to existing object structure without modification
- Collect related operations in visitor rather than scattering them across element classes

### Pattern Participants
- **Visitor**: Abstract interface declaring visit operation for each type of ConcreteElement
- **ConcreteVisitor**: Implements each operation declared by Visitor, defines context for algorithm
- **Element**: Abstract interface defining accept operation that takes visitor as argument
- **ConcreteElement**: Implements accept operation that typically calls back visitor method
- **ObjectStructure**: Enumerates elements and provides interface for visitor to visit elements

### Implementation Considerations
- Double dispatch mechanism enables operation selection based on both visitor and element type
- Adding new element types requires changing all visitor classes
- Visitors can accumulate state while traversing object structure
- ObjectStructure can be composite or collection providing element enumeration

## Key Points
- **Operation Extension**: New operations can be added without modifying existing element classes
- **Related Operations**: Operations that work across class hierarchy can be kept together in visitor
- **Double Dispatch**: Enables selection of appropriate operation based on both visitor type and element type being visited