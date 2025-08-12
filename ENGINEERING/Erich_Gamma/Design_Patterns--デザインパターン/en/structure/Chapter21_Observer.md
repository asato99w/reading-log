# Chapter 21: Observer (Behavioral)

## Chapter Overview
Defines a one-to-many dependency between objects so that when one object changes state, all dependents are notified and updated automatically.

## Main Content

### Intent and Structure
- Establish dynamic relationships between objects where multiple observers need notification of subject state changes
- Maintain loose coupling between subject and observers, allowing independent variation of both
- Enable broadcast communication where subject doesn't need to know specific observers
- Support dynamic addition and removal of observer relationships at runtime

### Pattern Participants
- **Subject**: Maintains list of observers and provides interface for attaching/detaching observer objects
- **Observer**: Defines updating interface for objects that should be notified of subject changes
- **ConcreteSubject**: Stores state of interest and sends notification to observers when state changes
- **ConcreteObserver**: Maintains reference to ConcreteSubject object and implements update interface to keep state consistent

### Implementation Considerations
- Push vs. pull notification models affect performance and flexibility trade-offs
- Observer registration and unregistration must be handled carefully to prevent memory leaks
- Update order may matter for some applications, requiring careful observer list management
- Complex update dependencies may require additional coordination mechanisms

## Key Points
- **Broadcast Communication**: Observer enables one-to-many communication where subject broadcasts changes to all registered observers without knowing their specific types
- **Loose Coupling**: Subject and observer are loosely coupled, with subject knowing only that observers implement update interface, enabling independent modification
- **Dynamic Relationships**: Observer relationships can be established and changed at runtime, providing flexibility for changing communication requirements