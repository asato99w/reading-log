# Chapter 22: State (Behavioral)

## Chapter Overview
Allows an object to alter its behavior when its internal state changes, appearing as if the object changed its class.

## Main Content

### Intent and Structure
- Allow object behavior to change based on internal state changes
- Eliminate large conditional statements for state-dependent behavior
- Make state transitions explicit through state objects
- Enable state-specific behavior while maintaining object identity

### Pattern Participants
- **Context**: Defines interface of interest to clients, maintains instance of ConcreteState subclass that defines current state
- **State**: Abstract interface for encapsulating behavior associated with particular state of Context
- **ConcreteState**: Each subclass implements behavior associated with state of Context

### Implementation Considerations
- Context delegates state-specific requests to current ConcreteState object
- State transitions can be controlled by State classes or Context class
- States can be shared if they don't have instance variables
- Creation and destruction of state objects affects performance and memory usage

## Key Points
- **Behavior Variation**: Object behavior changes based on current state without changing object class or identity
- **State Encapsulation**: Each state's behavior encapsulated in separate class, making code more maintainable
- **Explicit Transitions**: State changes are explicit and can be easily tracked and controlled