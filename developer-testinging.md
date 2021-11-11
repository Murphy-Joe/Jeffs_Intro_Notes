# Developer Testing


## Code Quality

Two Kinds:
- Internal
    How easy is it to change?
    - You probably aren't going to get it right the first time.
    - The two "metrics" associated with this are:
        1. Coupling - the strength of relationships between code modules
            You want LOW coupling
        2. Cohesion - how well things go together
            You want HIGH cohesion.
- External (to help with this, but need to taken with a grain of salt.)
    "Does it work? Does it meet the requirements?"
    Other people need to verify it.

## Types of Developer Tests
### Unit Tests
- Test a single "Unit" of code in isolation from other code.
- a Unit for us is usually a method on a class.
- These are "White Box" tests - they know how the code is implemented.

Unit tests can NEVER:
    - Touch a database
    - Touch the file system
    - Use the network
    - Interact with a user
    - Depend on a clock

    
### Isolated Integration Tests
- Anytime we are testing more than one unit together.
- You can only test your code.
    - You can't test other service

## Methodologies of Testing
### Test After
    - You write the code, and then you add some tests. 
    - I do this a lot with integration tests.
    - Pretty stupid to do with Unit tests.
### Test First
    - Just writing the test first.
### Test-Driven Development
    - Test First
    - A DESIGN methodology.

    "Discipline" of TDD:
    - Everything starts with a failing test.
    - Get that to pass quick.
        - ANYTHING GOES. Do not worry about writing "great" code.
        - If it takes you longer than *X* minutes, delete the test, and write another one.
    - Make it good. 

    Red -> Green -> Refactor


## Four Rules of Simple Design

Passes the tests
Reveals intention



No duplication (DRY - Don't Repeat Yourself - "Moist")
Fewest elements (Bugs scale linearly with the numbers of lines of code.)