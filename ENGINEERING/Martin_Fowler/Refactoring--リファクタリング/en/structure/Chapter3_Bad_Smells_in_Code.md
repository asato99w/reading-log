# Chapter 3: Bad Smells in Code

## Chapter Overview
This chapter, co-authored with Kent Beck, introduces the concept of "code smells" - symptoms in code that suggest refactoring opportunities. Rather than providing rules, it trains intuition for recognizing problematic code.

## Main Content
- **The 22 Code Smells**
  - Duplicated Code: Same code structure in multiple places
  - Long Method: Methods doing too much, hard to understand
  - Large Class: Classes with too many responsibilities
  - Long Parameter List: Methods with many parameters
  - Divergent Change: Class changed for multiple reasons
  - Shotgun Surgery: One change requires many small edits
  - Feature Envy: Method more interested in other class
  - Data Clumps: Same data groups appearing together
  - Primitive Obsession: Overuse of primitives instead of objects
  - Switch Statements: Type-based switching instead of polymorphism
  - Parallel Inheritance Hierarchies: Paired class hierarchies
  - Lazy Class: Class not doing enough to justify existence
  - Speculative Generality: Unnecessary abstraction
  - Temporary Field: Fields only used in certain circumstances
  - Message Chains: Long chains of method calls
  - Middle Man: Class only delegating to another
  - Inappropriate Intimacy: Classes knowing too much about each other
  - Alternative Classes with Different Interfaces: Similar classes with different methods
  - Incomplete Library Class: Library missing needed features
  - Data Class: Class with only data, no behavior
  - Refused Bequest: Subclass not using superclass features
  - Comments: Need for comments indicating unclear code

- **Smell Patterns and Relationships**
  - How smells compound and interact
  - Which smells are most serious
  - Context-dependent smell evaluation
  - Team-specific smell tolerances

## Key Points
- Code smells are intuitive rather than precise - develop a "nose" for problems
- Not all smells must be fixed immediately - prioritize based on change frequency
- The same smell might have different solutions in different contexts