# Chapter 10: ISP: Interface Segregation Principle

## Chapter Overview
This chapter shows how avoiding dependency on unused interfaces prevents unnecessary coupling, supporting architectural boundary definition and maintaining system flexibility.

## Main Content

### The Problem of Fat Interfaces
- Large interfaces with many methods force clients to depend on functionality they don't use
- Changes to unused interface methods can force recompilation and redeployment of unaffected clients
- Fat interfaces create unnecessary coupling between unrelated parts of the system
- Interface pollution occurs when interfaces grow to accommodate diverse client needs

### Segregating Interfaces by Client Needs
- Interfaces should be tailored to the specific needs of their clients rather than comprehensive feature sets
- Role interfaces focus on specific client requirements rather than complete object capabilities
- Interface segregation can be achieved through multiple inheritance of focused interfaces
- Adapter patterns can help retrofit existing fat interfaces with segregated alternatives

### Architectural Benefits of Interface Segregation
- Reduced coupling between system components through focused interface contracts
- Independent evolution of different interface aspects without affecting unrelated clients
- Cleaner dependency graphs that reflect actual usage patterns rather than comprehensive capabilities
- Improved testability through focused mock objects and test doubles

## Key Points
1. **Client-Specific Interfaces**: Interfaces should be designed around client needs rather than implementer capabilities
2. **Reduced Coupling**: Interface segregation minimizes dependencies and enables independent component evolution
3. **Architectural Clarity**: Segregated interfaces make system dependencies explicit and manageable