# Chapter 20: Business Rules

## Chapter Overview
This chapter distinguishes between critical business rules (entities) and application-specific business rules (use cases), forming the core of clean architecture and establishing the foundation for system organization.

## Main Content

### Critical Business Rules and Entities
- Critical business rules are rules that would exist even if the system were not automated
- Entities encapsulate the most general and high-level rules that define the core business concepts
- These rules are independent of any particular application or use case implementation
- Entities should have no dependencies on databases, user interfaces, or any other system concerns

### Application Business Rules and Use Cases
- Use cases contain application-specific business rules that define how the system behaves
- Use cases orchestrate the flow of data to and from entities while applying application-specific rules
- They specify user interactions with entities but remain independent of implementation details
- Use cases define the application's behavioral requirements without specifying technical implementation

### The Entity-Use Case Collaboration
- Use cases depend on entities, but entities know nothing about use cases
- This dependency direction protects the most critical business rules from application-specific changes
- Use cases manipulate entities through well-defined interfaces without violating entity encapsulation
- The collaboration enables reuse of entities across different applications and use cases

## Key Points
1. **Rule Hierarchy**: Critical business rules (entities) are more stable and important than application-specific rules (use cases)
2. **Independence**: Both entities and use cases should be independent of technical implementation details like databases and UI
3. **Collaboration Pattern**: Use cases orchestrate entities while maintaining proper dependency direction to protect business rules