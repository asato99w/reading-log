# Chapter 6: Equality for All, Redux

## Chapter Overview
Implementing equality for Franc objects and discovering that Dollar and Franc with the same amount are not equal. This creates the foundation for understanding when objects should be considered equal and begins to reveal the need for currency as part of equality.

## Main Content
- **Franc Equality Implementation**
  - Implementing equals() method for Franc class following same pattern as Dollar
  - Ensuring Franc objects compare correctly with each other
  - Establishing consistent equality behavior across both currency classes
  - Maintaining parallel implementation while preparing for consolidation

- **Cross-Currency Inequality**
  - Discovering that 5 dollars should not equal 5 francs
  - Understanding that equality must consider object type, not just value
  - Recognizing the need for currency as part of the equality calculation
  - Learning that different classes with same values may not be equal

- **Preparing for Consolidation**
  - Observing duplication between Dollar and Franc equals() methods
  - Understanding that similar implementations suggest common abstraction
  - Setting up the need for shared parent class or common behavior
  - Planning the path toward unified equality implementation

## Key Points
- Equality implementation must consider all relevant aspects of an object's identity, not just its primary value
- Objects of different types should typically not be equal, even if they have the same values
- Parallel implementations often reveal opportunities for abstraction and consolidation