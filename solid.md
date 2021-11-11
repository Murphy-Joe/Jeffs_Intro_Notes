# SOLID Principals

(See Steve Smith's pluralsight course as post-class refresher)

## Cohesion (how well things go together)
### Single Responsibility
Each "code module" (method, class, etc.) should have no more than one thing it does.

### Open Closed
"Code should be closed for modification but open for extension"
Write code so that after it works, you NEVER need to change it.


### Liskov Substitution
A type should be replaceable for it's subtype. (whatever that means)

## Coupling (the strength of relationships between things)
### Interface Segregation

- depend on small *client specific* interfaces.
### Dependency Inversion
- "Rely on Abstractions, Not Concretions"

My bank account NEEDS a thing to calculate bonuses, but it cannot CREATE it.


Bank Account -> Deposit -> StandardBonusCalculaor

Bonus Calculator -> BankAccount -> Deposit