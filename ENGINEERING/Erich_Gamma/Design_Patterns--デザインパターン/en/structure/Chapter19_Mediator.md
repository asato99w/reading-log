# Chapter 19: Mediator (Behavioral)

## Chapter Overview
Defines how a set of objects interact with each other through a mediator object that promotes loose coupling by keeping objects from referring to each other explicitly.

## Main Content

### Intent and Structure
- Define how set of objects interact without them referring to each other explicitly
- Promote loose coupling by keeping objects from knowing about each other directly
- Centralize complex communications and control logic between related objects
- Enable reuse of individual colleague objects by separating interaction logic

### Pattern Participants
- **Mediator**: Interface for communication between Colleague objects
- **ConcreteMediator**: Implements cooperative behavior by coordinating Colleague objects
- **Colleague**: Classes that communicate with other colleagues through Mediator

### Implementation Considerations
- Mediator can become complex if it handles too much interaction logic
- Abstract mediator may not be needed if only one concrete mediator exists
- Colleagues can communicate with mediator using Observer pattern
- Mediator can be implemented as Singleton if only one instance needed

## Key Points
- **Centralized Communication**: All inter-object communication goes through mediator, centralizing interaction logic
- **Loose Coupling**: Colleagues don't reference each other directly, reducing dependencies between objects
- **Interaction Control**: Mediator controls and coordinates interactions, enabling complex communication protocols