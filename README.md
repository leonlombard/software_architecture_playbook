# Software Architecture Playbook

## Refactoring

### Refactor code using the Strangler pattern

This includes the following steps:

1. Define an Interface for the Thing That Needs to Be Extracted
2. Change Calls to the Old System to Use the New System Instead
3. Make a New Data Source for the New System If It Requires Writing
4. Implement Writers in the New Model to Write to the New Data Source
5. Backfill the New Data Source with Existing Data
6. Change the Methods in the Newly Defined Interface to Read Data from the New Source
7. Stop Writing to the Old Source and Delete Legacy Code

### Resources

- Article: [Strangler Fig by Martin Fowler](https://martinfowler.com/bliki/StranglerFigApplication.html)
- Artilce: [Refactoring Legacy Code with the Strangler Fig Pattern by Adrianna Chang](https://shopify.engineering/refactoring-legacy-code-strangler-fig-pattern)
