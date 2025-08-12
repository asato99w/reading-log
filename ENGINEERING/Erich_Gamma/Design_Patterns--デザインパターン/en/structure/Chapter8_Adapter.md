# Chapter 8: Adapter (Structural)

## Chapter Overview
Allows classes with incompatible interfaces to work together by wrapping one class with an adapter that translates interface calls.

## Main Content

### Intent and Structure
- Allow collaboration between classes with incompatible interfaces
- Wrap existing class with new interface without modifying original code
- Enable reuse of existing classes when their interfaces don't match requirements
- Convert interface of class into another interface clients expect

### Pattern Participants
- **Target**: Interface that client expects to work with
- **Adaptee**: Existing class with incompatible interface that needs adapting
- **Adapter**: Implements Target interface and translates calls to Adaptee
- **Client**: Collaborates with objects conforming to Target interface

### Implementation Variations
- **Object Adapter**: Uses composition to wrap Adaptee instance and translate calls
- **Class Adapter**: Uses inheritance to adapt interface, requires multiple inheritance
- **Two-way Adapter**: Can act as both Target and Adaptee, enabling bidirectional adaptation

### Implementation Considerations
- Object adapter more flexible but requires forwarding all Target methods to Adaptee
- Class adapter can override Adaptee behavior but ties Adapter to specific Adaptee class
- Amount of adaptation required affects complexity of Adapter implementation

## Key Points
- **Interface Translation**: Adapter enables collaboration between classes with incompatible interfaces without modifying existing code
- **Legacy Integration**: Particularly valuable for integrating legacy systems with new code that expects different interfaces
- **Third-party Integration**: Enables use of third-party libraries when their interfaces don't match application requirements