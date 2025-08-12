# Chapter 14: Maintaining Model Integrity

## Chapter Overview
Introduces Bounded Context and Context Map patterns for managing multiple models within large systems and addressing integration challenges.

## Main Content

### Bounded Context Fundamentals
- Explicit boundaries define where specific domain models apply and remain internally consistent
- Different contexts may have different models of same business concepts based on their specific needs
- Context boundaries enable teams to work independently while managing integration complexity
- Clear context definition prevents model corruption through inappropriate concept mixing

### Context Map Patterns
- Shared Kernel allows multiple contexts to share common model elements with coordinated evolution
- Customer-Supplier relationships define upstream/downstream dependencies between contexts
- Anticorruption Layer protects downstream context from upstream model changes and concepts
- Separate Ways acknowledges that some integration costs exceed benefits and contexts should remain independent

### Integration Strategy Selection
- Context relationship patterns should be chosen based on organizational and technical constraints
- Integration overhead must be balanced against benefits of shared understanding
- Different integration patterns may be appropriate for different context pairs within same system
- Context boundaries and integration patterns should evolve as organizational and system needs change

## Key Points
- **Explicit Boundaries**: Bounded contexts provide essential tool for managing model complexity in large systems by defining clear scope limitations
- **Integration Patterns**: Context mapping provides vocabulary for describing and managing relationships between different domain models
- **Organizational Alignment**: Context boundaries should align with team and organizational structures to minimize coordination overhead