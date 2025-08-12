# Chapter 20: Memento (Behavioral)

## Chapter Overview
Captures and externalizes an object's internal state so that the object can be restored to this state later without violating encapsulation.

## Main Content

### Intent and Structure
- Capture object's internal state without violating encapsulation
- Enable object restoration to previous state for undo functionality
- Provide snapshot capability for objects with complex internal state
- Support checkpointing and rollback operations in applications

### Pattern Participants
- **Originator**: Creates memento containing snapshot of its current internal state
- **Memento**: Stores internal state of Originator, protects against access by other objects
- **Caretaker**: Responsible for memento's safekeeping, never operates on or examines memento contents

### Implementation Considerations
- Memento should store only state necessary for restoration
- Wide interface available to Originator, narrow interface to other objects
- Caretaker manages memento lifecycle but doesn't access memento contents
- Memory overhead can be significant if mementos stored frequently

## Key Points
- **Encapsulation Preservation**: Internal state captured and restored without breaking object's encapsulation
- **Undo Functionality**: Enables sophisticated undo/redo mechanisms in applications
- **State Management**: Provides clean way to handle object state snapshots and restoration