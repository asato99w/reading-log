# Chapter 13: Component Cohesion

## Chapter Overview
This chapter explores the REP, CCP, and CRP principles for determining what belongs together in components, balancing reusability, maintainability, and stability concerns.

## Main Content

### The Reuse/Release Equivalence Principle (REP)
- The granule of reuse is the granule of release - components must be released and versioned as cohesive units
- Classes and modules that are reused together should be grouped together in the same component
- Release versioning enables users to decide when and how to adopt new versions of components
- REP ensures that reusable components have meaningful release boundaries and version management

### The Common Closure Principle (CCP)
- Gather into components those classes that change for the same reasons and at the same times
- CCP is the Single Responsibility Principle applied at the component level
- Components should be closed against the same kinds of changes that affect their constituent classes
- When change is necessary, it should be confined to a minimal number of components

### The Common Reuse Principle (CRP)
- Don't force users of a component to depend on things they don't need
- Classes that tend to be reused together should be grouped together in components
- CRP is the Interface Segregation Principle applied at the component level
- Components should not include classes that client components don't actually use

## Key Points
1. **Cohesion Tensions**: The three principles create tension between reusability (REP), maintainability (CCP), and stability (CRP) that must be balanced
2. **Change Management**: Proper component cohesion minimizes the impact of changes by localizing related modifications
3. **Release Strategy**: Component boundaries should align with release and versioning strategies to support effective dependency management