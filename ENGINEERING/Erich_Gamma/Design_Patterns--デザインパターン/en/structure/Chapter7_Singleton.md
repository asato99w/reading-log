# Chapter 7: Singleton (Creational)

## Chapter Overview
Ensures a class has only one instance and provides global access point to that instance.

## Main Content

### Intent and Structure
- Ensure that a class has exactly one instance throughout application lifetime
- Provide global access point to the single instance from anywhere in application
- Control instantiation process to prevent multiple instances from being created
- Manage shared resources that should have single point of access and control

### Pattern Participants
- **Singleton**: Class that maintains single instance of itself and provides global access through static method
- **Client**: Accesses Singleton instance through static getInstance() method rather than constructor

### Implementation Considerations
- Constructor must be private or protected to prevent external instantiation
- Thread safety requires careful consideration in multithreaded environments
- Lazy initialization vs. eager initialization affects performance and resource usage
- Subclassing singleton classes presents significant challenges and should generally be avoided

### Common Implementation Variations
- **Eager Initialization**: Create instance at class loading time, thread-safe but may waste resources
- **Lazy Initialization**: Create instance when first requested, requires thread synchronization
- **Thread-Safe Lazy**: Use synchronization mechanisms to ensure thread safety during lazy initialization
- **Double-Checked Locking**: Optimize thread-safe lazy initialization to reduce synchronization overhead

## Key Points
- **Single Instance Guarantee**: Singleton ensures only one instance exists, preventing resource conflicts and maintaining consistent state
- **Global Access**: Provides global access point that can be used from anywhere in application without passing references
- **Controlled Instantiation**: Class controls its own instantiation process, enabling lazy loading and resource management optimization