# Chapter 8: Makin' Objects

## Chapter Overview
Introducing factory methods to simplify object creation and prepare for further abstraction. Shows how TDD supports the introduction of creation patterns and how good naming can improve code readability and design.

## Main Content
- **Factory Method Introduction**
  - Creating static factory methods dollar() and franc() in Money class
  - Simplifying client code by hiding constructor complexity
  - Preparing for potential future changes in object creation
  - Understanding the Factory Method pattern in practice

- **Interface Simplification**
  - Making object creation more expressive through well-named factory methods
  - Reducing coupling between client code and specific classes
  - Creating more readable test code through better naming
  - Setting up flexibility for future implementation changes

- **Design Pattern Application**
  - Applying Factory Method pattern to improve design
  - Understanding when and why factory methods are useful
  - Balancing simplicity with flexibility in object creation
  - Preparing the codebase for further abstraction

## Key Points
- Factory methods can make code more readable and flexible by hiding construction details behind expressive method names
- Good naming in factory methods makes client code more intention-revealing and easier to understand
- Factory methods provide a layer of indirection that enables future changes to object creation without affecting clients