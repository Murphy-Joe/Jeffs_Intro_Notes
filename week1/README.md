# Summary of Week 1

"Getting to Know You"

A lot of getting used to Visual Studio, C#.

We talked a lot about **loose coupling** and **cohesion** in software.

Why?

## Loose Coupling

> Coupling is the strength of relationships between code modules (classes, functions, etc.)

Loose Coupling enables us to make small changes or additions to our systems without negatively impacting the rest of the system.

This is important for:
- Maintaining code over time
- CI/CD patterns

Loose Coupling is accomplished by:

### Interface Segregation 

> Depending on small, client-specific interfaces

"Interface" here means "the thing way a thing I need looks, as opposed to how it is implemented". (it's not coincidental that C# has an `interface` construct, but it could be an API interface, etc.)

### Dependency Inversion
> Rely on Abstractions, Not Concretions

That just means that a code module (class) can't know what particular "real" class is going to provide the functionality it needs.

This is also important for isolated integration testing, as you'll see.

We also emphasized *delegates*, because they are a way to depend on an abstraction. My `Filter` method relies on *something* that can tell it if a number should be included in the results or not, not a specific method.

Interfaces allow you to have multiple methods, related together in a contract.

A Delegate is just one method.

Delegates can be easier to work with because you don't need to create a class that implements it, etc.

## C# Details

Don't sweat it. You'll get it. You'll have to google stuff, no problem. 

## Unit Testing

Unit Testing and TDD were used in class to show you how to get to a loosely coupled, highly-cohesive system.

