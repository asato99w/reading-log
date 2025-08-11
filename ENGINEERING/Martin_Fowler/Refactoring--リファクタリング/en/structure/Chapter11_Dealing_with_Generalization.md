# Chapter 11: Dealing with Generalization

## Chapter Overview
This chapter addresses refactorings that work with inheritance hierarchies, moving features up and down the hierarchy to create better abstractions and eliminate duplication.

## Main Content
- **Moving Features in Hierarchy**
  - Pull Up Field: Move field used by subclasses to superclass
  - Pull Up Method: Move method with identical results on subclasses to superclass
  - Pull Up Constructor Body: Move common constructor code to superclass
  - Push Down Method: Move method relevant to only some subclasses down hierarchy
  - Push Down Field: Move field used by only some subclasses down hierarchy

- **Creating and Refining Abstractions**
  - Extract Subclass: Create subclass for subset of features used only by some instances
  - Extract Superclass: Create superclass when two classes have similar features
  - Extract Interface: Create interface when several clients use same subset of class's interface
  - Collapse Hierarchy: Merge superclass and subclass when they're not different enough

- **Template Method and Strategy Patterns**
  - Form Template Method: Create template method when subclasses do same thing in same order but different ways
  - Replace Inheritance with Delegation: Use delegation when subclass uses only part of superclass interface
  - Replace Delegation with Inheritance: Use inheritance when delegation becomes cumbersome with simple relationship

## Key Points
- Inheritance hierarchies should reflect genuine "is-a" relationships
- Common behavior belongs in superclasses, specialized behavior in subclasses
- Sometimes delegation is better than inheritance for code reuse