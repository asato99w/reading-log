# Chapter 6: The Life Cycle of a Domain Object

## Chapter Overview
Introduces patterns for managing domain object lifecycles: Aggregates for consistency boundaries, Factories for creation, and Repositories for retrieval.

## Main Content

### Aggregate Pattern
- Consistency boundary grouping related entities and value objects under single root
- Aggregate root serves as single entry point for external access and modification
- Internal aggregate consistency maintained through root's control of modifications
- Transactions should generally align with aggregate boundaries to ensure business invariant preservation

### Factory Pattern
- Encapsulates complex object creation logic while maintaining domain focus
- Factories ensure newly created objects satisfy all business invariants and constraints
- Creation logic may be embedded in aggregate roots, separate factory objects, or factory methods
- Factories should produce fully formed, valid domain objects ready for use

### Repository Pattern
- Provides collection-like interface for accessing existing domain objects
- Encapsulates data access concerns while presenting domain-focused query interface
- Repositories should return fully reconstituted domain objects, not data transfer objects
- Query methods should use domain language and concepts rather than technical database terminology

## Key Points
- **Aggregate Boundaries**: Aggregates define consistency boundaries that align business invariants with technical transaction boundaries
- **Creation Encapsulation**: Factories hide complex creation logic while ensuring all created objects meet domain requirements and business rules
- **Access Abstraction**: Repositories provide domain-focused access to persistent objects while hiding infrastructure complexity from domain logic