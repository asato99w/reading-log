# Chapter 21: Screaming Architecture

## Chapter Overview
This chapter advocates for architectures that clearly communicate their purpose and domain intent rather than their technical implementation choices, making business requirements immediately visible in system structure.

## Main Content

### Architecture Should Scream Its Purpose
- The architecture of a system should immediately reveal what the system does, not what frameworks it uses
- A library architecture should scream "library," a healthcare system should scream "healthcare"
- Top-level directory structure should reflect use cases and business concepts, not technical layers
- The most important architectural elements should be the most visible in the system structure

### Framework-Centric vs. Domain-Centric Architecture
- Framework-centric architectures organize around technical concerns (MVC directories, database layers)
- Domain-centric architectures organize around business concepts (patient management, book lending)
- Frameworks are tools to be used by the architecture, not the determining factor of architectural structure
- Business logic should be clearly separated and highlighted, not buried within framework-specific directories

### Making Use Cases Visible
- Use cases should be first-class architectural citizens with clear representation in the codebase
- Each use case should have a clear implementation that can be found easily by developers
- The architecture should make it obvious what the system does for its users
- Technical details should be subordinate to business functionality in architectural prominence

## Key Points
1. **Purpose Visibility**: System architecture should immediately communicate what the system does rather than how it's implemented
2. **Business-First Organization**: Directory structure and component organization should reflect business concepts over technical frameworks
3. **Use Case Prominence**: Use cases should be clearly visible and easily discoverable within the architectural structure