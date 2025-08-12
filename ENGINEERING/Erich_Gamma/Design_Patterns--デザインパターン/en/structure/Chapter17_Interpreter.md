# Chapter 17: Interpreter (Behavioral)

## Chapter Overview
Defines a representation for grammar of a language and an interpreter that uses the representation to interpret sentences in the language.

## Main Content

### Intent and Structure
- Define grammar representation for simple language and build interpreter for that grammar
- Use when language statements can be represented as abstract syntax trees
- Enable interpretation of sentences in defined language through grammar rules
- Support languages where grammar is simple and efficiency is not primary concern

### Pattern Participants
- **AbstractExpression**: Interface for executing operation common to all nodes in abstract syntax tree
- **TerminalExpression**: Implements interpret operation for terminal symbols in grammar
- **NonterminalExpression**: Implements interpret operation for nonterminal symbols, maintains references to other expressions
- **Context**: Contains information global to interpreter, passed to each expression during interpretation
- **Client**: Builds abstract syntax tree and invokes interpret operation

### Implementation Considerations
- Each grammar rule becomes a class in the implementation
- Abstract syntax tree built by client before interpretation begins
- Context object can store global state and provide services to expressions
- Visitor pattern can be used to add new operations without changing expression classes

## Key Points
- **Grammar Representation**: Each grammar rule is represented by a class, making language structure explicit in code
- **Composable Interpretation**: Complex expressions built by composing simpler expressions following grammar rules
- **Domain-Specific Languages**: Particularly useful for implementing domain-specific languages and expression evaluators