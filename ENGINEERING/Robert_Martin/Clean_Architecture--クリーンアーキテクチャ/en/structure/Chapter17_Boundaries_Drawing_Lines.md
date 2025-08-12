# Chapter 17: Boundaries: Drawing Lines

## Chapter Overview
This chapter demonstrates how to identify and implement architectural boundaries, separating high-level policies from low-level details through strategic architectural line-drawing.

## Main Content

### Identifying Architectural Boundaries
- Boundaries separate components with different rates of change and different reasons for change
- The most important boundaries separate business rules from technical implementation details
- Database boundaries, UI boundaries, and external service boundaries protect core business logic
- Boundaries should be drawn where the architecture wants to preserve the ability to make decisions later

### The Single Responsibility Principle at Architectural Scale
- Different actors (stakeholders) who request changes should be separated by architectural boundaries
- Business rules serve business actors and should be separated from technical infrastructure concerns
- User interface components serve users and should be separated from business rule implementations
- Data persistence serves operational requirements and should be separated from business logic

### Implementing Boundary Crossing
- Boundaries are crossed using simple data structures or function calls, not complex objects
- Data that crosses boundaries should be in simple, serializable formats
- Control flow can cross boundaries, but source code dependencies must respect the boundary direction
- Plugins and adapters are common patterns for implementing clean boundary crossings

## Key Points
1. **Change Rate Boundaries**: Architectural boundaries should separate components that change at different rates and for different reasons
2. **Actor Separation**: Different stakeholders should be separated by boundaries to prevent coupling between unrelated concerns
3. **Simple Boundary Crossing**: Clean boundaries are crossed with simple data structures, maintaining architectural integrity