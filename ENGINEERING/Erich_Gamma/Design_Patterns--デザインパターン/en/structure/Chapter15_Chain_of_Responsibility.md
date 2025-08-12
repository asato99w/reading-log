# Chapter 15: Chain of Responsibility (Behavioral)

## Chapter Overview
Passes requests along a chain of handlers until one of them handles the request, decoupling sender from receiver.

## Main Content

### Intent and Structure
- Avoid coupling sender of request to its receiver by giving multiple objects chance to handle request
- Chain receiving objects and pass request along chain until object handles it
- Allow dynamic configuration of handler chain without modifying individual handlers
- Enable multiple objects to handle same request type based on runtime conditions

### Pattern Participants
- **Handler**: Interface for handling requests and accessing successor in chain
- **ConcreteHandler**: Handles requests it's responsible for, can access its successor
- **Client**: Initiates request to ConcreteHandler object on chain

### Implementation Considerations
- Handler can either handle request or forward it to successor in chain
- Request can be handled by exactly one handler or multiple handlers in sequence
- Chain configuration can be static (compile-time) or dynamic (runtime)
- Chain termination handled by either explicit end marker or null successor

### Chain Variations
- Pure chain where each handler either handles completely or passes on
- Partial handling where multiple handlers can process same request
- Broadcasting where request sent to all handlers regardless of handling

## Key Points
- **Decoupled Communication**: Sender doesn't need to know which object will handle request or how many objects are in chain
- **Dynamic Chain Configuration**: Handler chain can be configured at runtime to change request processing behavior
- **Flexible Request Handling**: Multiple objects can potentially handle request, and handling logic can be distributed across chain