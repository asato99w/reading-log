# Chapter 3: Bad Smells in Code

## Chapter Overview
This chapter updates the classic code smells catalog with JavaScript examples and introduces new smells specific to modern web development, including framework-specific anti-patterns and asynchronous programming issues.

## Main Content
- **Classic Smells with Modern Examples**
  - Duplicated Code: Module and API call duplication patterns
  - Long Function: Async/await complexity and ES6+ simplification opportunities
  - Large Class: ES6 classes and React component responsibility overload
  - Long Parameter List: Destructuring and default parameters improvement opportunities

- **Modern Web Development Smells**
  - Callback Hell: Async/await improvement opportunities
  - Global State Abuse: Proper state management pattern needs
  - Monolithic Components: Responsibility separation and component splitting
  - API Design Inconsistencies: RESTful patterns and unified error handling

- **Framework-Specific Smells**
  - React: useEffect dependency array issues, prop drilling
  - Vue.js: Reactivity misuse, excessive watchers
  - Angular: Dependency injection complexity, circular dependencies

## Key Points
- JavaScript-specific smell patterns enable more effective refactoring strategies
- Modern web frameworks introduce new forms of traditional smells requiring updated solutions
- Automated tools (ESLint, etc.) enable continuous smell detection and prevention