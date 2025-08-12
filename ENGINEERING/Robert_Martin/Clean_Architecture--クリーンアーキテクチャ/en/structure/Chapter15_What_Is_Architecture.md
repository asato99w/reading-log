# Chapter 15: What Is Architecture?

## Chapter Overview
This chapter defines architecture's purpose as facilitating development, deployment, operation, and maintenance while preserving options for future change and minimizing lifetime costs.

## Main Content

### The Purpose of Software Architecture
- Architecture's primary purpose is to support the life cycle of the system by minimizing lifetime cost and maximizing programmer productivity
- Good architecture makes systems easy to understand, develop, maintain, and deploy
- Architecture should preserve options and delay irreversible decisions as long as possible
- The ultimate goal is to minimize human resources required to build and maintain the system

### Development, Deployment, Operation, and Maintenance
- **Development**: Architecture should enable teams to develop efficiently without interfering with each other
- **Deployment**: The system should be deployable with a single action, without manual processes or complex procedures
- **Operation**: Architecture should make operational requirements clear and support necessary performance characteristics
- **Maintenance**: The most expensive aspect of software systems, architecture should make changes easy and safe

### Keeping Options Open
- Good architecture maximizes the number of decisions not made by deferring details as long as possible
- Policy (business rules) should be separated from details (databases, frameworks, devices) to preserve flexibility
- The longer you wait to make detail decisions, the more information you have to make them correctly
- Architecture should make it possible to change details without affecting high-level policy

## Key Points
1. **Lifecycle Support**: Architecture serves the entire system lifecycle from development through maintenance by reducing complexity and cost
2. **Option Preservation**: Good architecture delays irreversible decisions and maintains flexibility to adapt to changing requirements
3. **Policy-Detail Separation**: The core architectural insight is separating high-level business policies from low-level implementation details