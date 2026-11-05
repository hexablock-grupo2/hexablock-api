# Extensibility guide — supporting a new `gameId`

> The backend is documented to the same level as the game client (§3.1 of the project statement applies to it by the professor's guidance).
> Must reference **real classes and files**. Keep this document true: if a PR breaks one of these steps, the PR must update it.

![Extensibility diagram](diagrams/img/extensibility-diagram.png)

## Worked example: `hexa-fill` (the fifth variant of the game client)

### 1. Files to CREATE

| # | File | Implements / extends | Layer |
| --- | --- | --- | --- |
| 1 | TODO (`gameId` level section) | TODO | Entities |
| 2 | TODO (level section validation) | TODO | TODO |
| 3 | TODO (leaderboard ranking policy, only if it differs) | TODO | Entities |

### 2. Files to MODIFY (should be configuration/registration only)

| File | Change | Why it does not violate OCP |
| --- | --- | --- |
| TODO (composition root / registry) | Register the new `gameId` | TODO |

### 3. Files that must NOT change

- TODO: generic progress, leaderboard and level use cases, repositories, controllers, AOP decorators...

### 4. Tests to add

- TODO

## Small rule variations

| Variation | Where it goes | Files touched |
| --- | --- | --- |
| New leaderboard ranking policy | TODO | TODO |
| New field in a level section | TODO | TODO |

## Swapping an infrastructure adapter

Any infrastructure piece must be replaceable without the inner layers noticing. Each swap creates a new adapter for an existing port and changes only the composition root or configuration.

| Piece | Port | Current adapter | Files to create | Files to change |
| --- | --- | --- | --- | --- |
| Database | TODO | TODO | TODO | TODO |
| Password hashing / token signing | TODO | TODO | TODO | TODO |
| Deployment provider | n/a (configuration) | TODO | TODO | TODO |

The port's contract test suite must pass against the new adapter before the swap counts as done.
