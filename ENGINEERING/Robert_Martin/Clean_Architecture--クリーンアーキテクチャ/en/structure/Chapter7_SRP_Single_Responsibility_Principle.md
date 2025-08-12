# Chapter 7: SRP: Single Responsibility Principle

## Chapter Overview
This chapter clarifies the Single Responsibility Principle as separation of concerns for different actors rather than just single functionality, providing the foundation for cohesive architectural components.

## Main Content

### Understanding the True Meaning of SRP
- SRP is commonly misunderstood as "a function should do one thing" but actually means "a module should have one reason to change"
- The principle is about separating code that different actors depend upon to avoid coupling between unrelated concerns
- A module should be responsible to one, and only one, actor (a group of users or stakeholders)
- Violation occurs when code serves multiple actors, leading to unexpected changes affecting unrelated stakeholders

### Common SRP Violations and Their Problems
- Employee class handling business rules, persistence, and formatting serves multiple actors (HR, accounting, IT)
- Changes for one actor can inadvertently break functionality needed by other actors
- Merge conflicts arise when different teams modify the same class for different reasons
- Testing becomes complex when multiple concerns are mixed in single modules

### Applying SRP at Different Levels
- Function level: Each function should have a single, well-defined purpose
- Class level: Classes should serve a single actor with cohesive responsibilities  
- Module level: Modules should encapsulate functionality for one stakeholder group
- Component level: Components should serve related use cases for consistent actor groups

## Key Points
1. **Actor-Centric Design**: SRP is about organizing code around the people or groups who will request changes, not just functional decomposition
2. **Change Isolation**: Proper SRP application ensures that changes for one actor don't inadvertently affect other actors' functionality
3. **Cohesive Modules**: Following SRP creates modules with high internal cohesion and clear external interfaces