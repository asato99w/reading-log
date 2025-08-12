# Chapter 16: Command (Behavioral)

## Chapter Overview
Encapsulates a request as an object, allowing you to parameterize clients with different requests, queue operations, and support undo functionality.

## Main Content

### Intent and Structure
- Encapsulate requests as objects to enable parameterization of clients with different requests
- Queue, schedule, and log requests for later execution or persistence
- Support undo operations by storing command state and implementing reverse operations
- Decouple object that invokes operation from object that performs the operation

### Pattern Participants
- **Command**: Interface declaring execution method for performing operation
- **ConcreteCommand**: Implements Command interface and defines binding between Receiver and action
- **Receiver**: Object that performs actual work when command is executed
- **Invoker**: Asks command to carry out request without knowing specific command or receiver
- **Client**: Creates ConcreteCommand object and sets its receiver

### Implementation Considerations
- Commands can store state necessary for execution and undo operations
- Macro commands can combine multiple commands for complex operations
- Command history enables undo/redo functionality through command stack management
- Commands can be serialized for persistence, logging, or network transmission

### Advanced Applications
- **Queuing**: Commands can be queued for batch processing or scheduled execution
- **Logging**: Command execution can be logged for audit trails or crash recovery
- **Transactions**: Commands can be grouped into transactions with commit/rollback semantics
- **Remote Execution**: Commands can be transmitted across network boundaries

## Key Points
- **Request Encapsulation**: Command encapsulates all information needed to perform operation, including method name, receiver, and parameters
- **Decoupling**: Invoker is decoupled from receiver, knowing only about command interface, enabling flexible request handling
- **Undo Support**: Commands can store state necessary for undo operations, enabling sophisticated undo/redo functionality in applications