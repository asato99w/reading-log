# Chapter 9: LSP: Liskov Substitution Principle

## Chapter Overview
This chapter establishes substitutability requirements for polymorphism to work correctly, ensuring that architectural contracts remain stable across different implementations and maintaining system reliability.

## Main Content

### Understanding Substitutability Requirements
- Objects of a superclass should be replaceable with objects of a subclass without breaking application functionality
- LSP defines the behavioral contract that subtypes must honor to maintain system correctness
- Substitutability goes beyond syntactic correctness to include semantic and behavioral compatibility
- Violations of LSP often indicate design flaws in inheritance hierarchies and abstraction choices

### Common LSP Violations and Their Impact
- Subclasses that strengthen preconditions or weaken postconditions violate client expectations
- Runtime type checking (instanceof, downcasting) often indicates LSP violations in the design
- Exception throwing in subclasses for operations that shouldn't fail violates the behavioral contract
- Side effects in subclasses that aren't present in the superclass can break client code assumptions

### LSP and Interface Design
- Well-designed interfaces embody the behavioral contracts that implementations must honor
- Interface segregation helps avoid LSP violations by creating more focused behavioral contracts
- Design by contract principles support LSP by making behavioral expectations explicit
- Testing strategies should verify that all implementations satisfy the same behavioral contracts

## Key Points
1. **Behavioral Contracts**: LSP ensures that abstractions maintain consistent behavioral contracts across all implementations
2. **Polymorphism Reliability**: Proper LSP adherence makes polymorphism safe and predictable in architectural designs
3. **Design Quality Indicator**: LSP violations often reveal problems in abstraction design that need architectural attention