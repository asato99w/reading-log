# CLAUDE.md - Clean Architecture Reading Log Project

## Project Overview
This is a reading log project for "Clean Architecture: A Craftsman's Guide to Software Structure and Design" by Robert C. Martin (Uncle Bob). Published in 2017, this influential work provides comprehensive guidance on software architecture principles that emphasize independence from frameworks, databases, and external concerns while prioritizing long-term maintainability.

## Work Information
- **Title**: Clean Architecture: A Craftsman's Guide to Software Structure and Design
- **Author**: Robert Cecil Martin (Uncle Bob)
- **Japanese Title**: クリーンアーキテクチャ
- **Original Publication**: September 2017 (Prentice Hall)
- **Japanese Publication**: July 2018 (KADOKAWA)
- **Japanese Translator**: 角征典、高木正弘
- **Pages**: 432 pages (English edition)
- **ISBN**: 978-0134494166 (English), 978-4048930659 (Japanese)

## Book Structure
The book is organized into six main parts with 34 chapters:

### Part I: Introduction (Chapters 1-2)
- Chapter 1: What Is Design and Architecture?
- Chapter 2: A Tale of Two Values

### Part II: Starting with the Bricks: Programming Paradigms (Chapters 3-6)
- Chapter 3: Paradigm Overview
- Chapter 4: Structured Programming
- Chapter 5: Object-Oriented Programming
- Chapter 6: Functional Programming

### Part III: Design Principles (Chapters 7-11)
- Chapter 7: SRP: The Single Responsibility Principle
- Chapter 8: OCP: The Open-Closed Principle
- Chapter 9: LSP: The Liskov Substitution Principle
- Chapter 10: ISP: The Interface Segregation Principle
- Chapter 11: DIP: The Dependency Inversion Principle

### Part IV: Component Principles (Chapters 12-19)
- Chapter 12: Components
- Chapter 13: Component Cohesion
- Chapter 14: Component Coupling
- Chapter 15: What Is Architecture?
- Chapter 16: Independence
- Chapter 17: Boundaries: Drawing Lines
- Chapter 18: Boundary Anatomy
- Chapter 19: Policy and Level

### Part V: Architecture (Chapters 20-23)
- Chapter 20: Business Rules
- Chapter 21: Screaming Architecture
- Chapter 22: The Clean Architecture
- Chapter 23: Presenters and Humble Objects

### Part VI: Details (Chapters 24-34)
- Chapter 24: Partial Boundaries
- Chapter 25: Layers and Boundaries
- Chapter 26: The Main Component
- Chapter 27: Services: Great and Small
- Chapter 28: The Test Boundary
- Chapter 29: Clean Embedded Architecture
- Chapter 30: The Database Is a Detail
- Chapter 31: The Web Is a Detail
- Chapter 32: Frameworks Are Details
- Chapter 33: Case Study: Video Sales
- Chapter 34: The Missing Chapter

## Key Learning Objectives
- Understanding the distinction between architecture and design, and their unified nature
- Mastering SOLID principles as the foundation for clean, maintainable systems
- Learning to manage dependencies strategically to support system evolution
- Developing skills for creating testable architectures that separate concerns effectively
- Building expertise in identifying and implementing appropriate architectural boundaries
- Understanding how to maintain business logic independence from technical implementation details

## Core Architectural Concepts
### Clean Architecture Principles
- **Independence of Frameworks**: Architecture doesn't depend on feature-laden frameworks
- **Testable**: Business rules can be tested without UI, database, web server, or external elements
- **Independence of UI**: UI can change without changing rest of system
- **Independence of Database**: Business rules not bound to specific database
- **Independence of External Agencies**: Business rules don't know about outside world

### SOLID Principles
- **Single Responsibility Principle**: Classes should have single reason to change
- **Open-Closed Principle**: Open for extension, closed for modification
- **Liskov Substitution Principle**: Objects of superclass should be replaceable with objects of subclass
- **Interface Segregation Principle**: Clients shouldn't depend on interfaces they don't use
- **Dependency Inversion Principle**: Depend on abstractions, not concretions

### Component Organization
- **Component Cohesion**: REP, CCP, CRP principles for what belongs together
- **Component Coupling**: ADP, SDP, SAP principles for managing dependencies
- **Architectural Boundaries**: Separating high-level policies from low-level details

## Implementation Notes
Follow the established repository structure with bilingual content organization. Focus on the practical application of architectural principles in modern software development contexts, including microservices, cloud-native applications, and distributed systems. Each chapter should emphasize both theoretical understanding and practical implementation strategies.

## Contemporary Relevance
Clean Architecture principles remain highly applicable to:
- **Microservices Architecture**: Service boundary design and dependency management
- **Cloud-Native Development**: Container-based applications and serverless architectures
- **DevOps Integration**: CI/CD pipeline design and infrastructure as code
- **Legacy System Modernization**: Systematic approaches to refactoring monolithic systems
- **AI/ML Integration**: Maintaining architectural boundaries when incorporating machine learning models

## Author Context
Robert C. Martin, known as "Uncle Bob," is a legendary figure in software development with over 50 years of programming experience. He co-authored the Agile Manifesto, founded Clean Coders, and has significantly influenced modern software engineering practices through his emphasis on craftsmanship, professionalism, and clean code principles.

## Related Works in Repository
- Domain-Driven Design by Eric Evans (complementary domain modeling approaches)
- Design Patterns by Gang of Four (foundational design patterns that align with clean architecture)
- Refactoring by Martin Fowler (systematic code improvement techniques)
- Test-Driven Development by Kent Beck (testing practices that support clean architecture)

## Analysis Focus Areas
When analyzing this work, emphasize:
- Practical application strategies for different system scales and contexts
- Trade-offs between architectural purity and development velocity
- Integration with modern development practices and tooling
- Adaptation of principles across different programming paradigms and languages
- Long-term system evolution and maintenance considerations