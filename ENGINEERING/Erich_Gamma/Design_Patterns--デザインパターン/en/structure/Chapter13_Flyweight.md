# Chapter 13: Flyweight (Structural)

## Chapter Overview
Uses sharing to support large numbers of fine-grained objects efficiently by separating intrinsic state from extrinsic state.

## Main Content

### Intent and Structure
- Support large numbers of objects efficiently by sharing common state
- Minimize memory usage when dealing with many similar objects
- Separate intrinsic state (shareable) from extrinsic state (context-dependent)
- Use shared flyweight objects configured with extrinsic state when needed

### Pattern Participants
- **Flyweight**: Interface through which flyweights can receive and act on extrinsic state
- **ConcreteFlyweight**: Implements Flyweight and stores intrinsic state, must be shareable
- **UnsharedConcreteFlyweight**: Not all flyweight subclasses need to be shared
- **FlyweightFactory**: Creates and manages flyweight objects, ensures flyweights are shared properly
- **Context**: Maintains reference to flyweight and stores extrinsic state

### Implementation Considerations
- Flyweights must not store extrinsic state that varies with context
- Extrinsic state passed as parameters to flyweight operations when needed
- Factory ensures that flyweights are shared and manages flyweight pool
- Client is responsible for maintaining extrinsic state and passing it to flyweight operations

## Key Points
- **Memory Efficiency**: Flyweight dramatically reduces memory usage when many similar objects are needed
- **State Separation**: Clear separation between intrinsic (shared) and extrinsic (context-dependent) state enables efficient sharing
- **Scalability**: Pattern enables applications to support very large numbers of objects that would otherwise consume prohibitive memory