# Chapter 19: Policy and Level

## Chapter Overview
This chapter establishes how to organize software components by their distance from inputs and outputs, creating stable architectural hierarchies that support system understanding and evolution.

## Main Content

### Defining Level in Software Architecture
- Level is defined by distance from inputs and outputs - components furthest from I/O are highest level
- Higher-level components contain business rules and policies that are central to the system's purpose
- Lower-level components handle details like user interfaces, databases, and external system integration
- Level provides an objective measure for organizing components in architectural hierarchies

### The Level Structure of Clean Architecture
- Business entities are highest level because they are furthest from inputs and outputs
- Use cases are lower level because they interact with entities but are closer to specific I/O scenarios  
- Interface adapters are lower still because they directly handle input and output formatting
- Frameworks and drivers are lowest level because they directly interface with external systems

### Dependency Direction and Architectural Stability
- Dependencies should point from lower level toward higher level components
- Higher-level components should not depend on lower-level components or their details
- Stable architectures have their most important business rules at the highest levels
- Changes flow downward in the level hierarchy, protecting important business policies

## Key Points
1. **Distance from I/O**: Component level is determined by distance from system inputs and outputs, with business rules being highest level
2. **Dependency Hierarchy**: Dependencies should flow from low-level details toward high-level policies to create stable architectures
3. **Business Rule Protection**: The most important business rules should be at the highest architectural levels, protected from lower-level changes