# Chapter 14: Proxy (Structural)

## Chapter Overview
Provides a surrogate or placeholder for another object to control access to it, enabling additional functionality without changing the original object.

## Main Content

### Intent and Structure
- Control access to another object by providing surrogate that acts as intermediary
- Add additional behavior (lazy loading, access control, caching) without modifying original object
- Provide location transparency for objects that may be in different address spaces
- Implement reference counting or other object lifecycle management

### Pattern Participants
- **Subject**: Common interface for RealSubject and Proxy, enabling Proxy to be used anywhere RealSubject is expected
- **RealSubject**: Real object that Proxy represents, defines real functionality
- **Proxy**: Maintains reference to RealSubject and controls access to it, implements same interface as RealSubject

### Proxy Types
- **Remote Proxy**: Provides local representative for object in different address space
- **Virtual Proxy**: Creates expensive objects on demand, implements lazy loading
- **Protection Proxy**: Controls access to original object based on access rights
- **Smart Reference**: Provides additional actions when object is accessed (reference counting, locking)

### Implementation Considerations
- Proxy interface should match Subject interface exactly for transparent substitution
- Proxy may need to create RealSubject instance if it doesn't exist (lazy loading)
- Copy-on-write proxies defer copying until modification is needed
- Reference management proxies track object usage and cleanup

## Key Points
- **Controlled Access**: Proxy provides controlled access to real object, enabling additional functionality like security or lazy loading
- **Transparent Substitution**: Proxy implements same interface as real object, enabling transparent replacement in client code
- **Location Independence**: Proxy can hide location details of real object, whether local, remote, or not yet created