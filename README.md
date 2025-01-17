# Software Architecture Playbook

## Deisgn Principles

These are a set of guidelines for helping guide how good quality software can be written. They include the following:

* Encapsulation
* Composition over inheritance
* Loose coupling
* Program to interfaces
* SOLID principles including:
  * Single responsibility principle
  * Open-closed principle
  * Liskov's substitution principle
  * Interface segregation principle
  * Dependency inversion principle

## Design Patterns

These provided a set of code structures that can be used to assist with adhering to design principles

## Refactoring

### Refactor code using the Strangler pattern

This includes the following steps:

1. Define an interface for the thing that needs to be extracted
2. Change calls to the old system to use the new system instead
3. Make a new data source for the new system if it requires writing
4. Implement writers in the new model to write to the new data source
5. Backfill the new data source with existing data
6. Change the methods in the newly defined interface to read data from the new source
7. Stop writing to the old source and delete legacy code

### Resources

- Article: [Strangler Fig by Martin Fowler](https://martinfowler.com/bliki/StranglerFigApplication.html)
- Artilce: [Refactoring Legacy Code with the Strangler Fig Pattern by Adrianna Chang](https://shopify.engineering/refactoring-legacy-code-strangler-fig-pattern)
