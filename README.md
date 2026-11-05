# HexaBlock Suite — Backend API

<!-- Badges: replace OWNER/REPO once the repo exists. CI badge appears after the first workflow run. -->
![commitlint](https://github.com/OWNER/REPO/actions/workflows/commitlint.yml/badge.svg)
<!-- TODO: build/test badge, test types badges, license badge -->

> REST API for HexaBlock Suite: users (JWT), progress per `gameId`, leaderboards and level definitions.

## Table of contents

- [Description](#description)
- [Architecture](#architecture)
- [Generic Engine](#generic-engine)
- [Design Patterns](#design-patterns)
- [SOLID Principles](#solid-principles)
- [AOP](#aop)
- [API Documentation](#api-documentation)
- [Getting Started](#getting-started)
- [Running Tests](#running-tests)
- [AI Usage Documentation](#ai-usage-documentation)
- [Contributing](#contributing)
- [License](#license)

## Description

TODO: what it is, what it is for, technologies used.

## Architecture

TODO: Clean Architecture explanation (4 layers, dependency rule, ports & adapters).

![Clean Architecture layers](docs/diagrams/img/clean-architecture-layers.png)

![Class diagram](docs/diagrams/img/class-diagram.png)

Editable source: [`docs/diagrams/src/`](docs/diagrams/src/)

How to support a new `gameId` or swap an infrastructure adapter: see [`docs/EXTENSIBILITY.md`](docs/EXTENSIBILITY.md).

## Generic Engine

The generic game engine lives in the [game client repository](https://github.com/hexablock-grupo2/hexablock-app). This section covers how the backend stays generic over `gameId`.

### One model per concept, one section per `gameId`

TODO: one progress, leaderboard and level model, with a `gameId`-specific section in the level schema (§5.2.4 of the statement).

### Generic types and bounded constraints

| Generic | Type parameters | Constraint | Reason |
| --- | --- | --- | --- |
| TODO | TODO | TODO | TODO |

How to support a new `gameId`: see [`docs/EXTENSIBILITY.md`](docs/EXTENSIBILITY.md).

## Design Patterns

| Category | Pattern | Where (link to code) | Why |
| --- | --- | --- | --- |
| Creational | TODO | TODO | TODO |
| Structural | TODO | TODO | TODO |
| Behavioural | TODO | TODO | TODO |

## SOLID Principles

TODO: one subsection per principle with a real code excerpt, the class/module and the justification.

## AOP

TODO: aspects implemented, decorator/proxy strategy over the generic use cases, why no library is used.

## API Documentation

TODO: Swagger / OpenAPI URL when running locally, and the path of the spec file.

| Method | Path | Description | Auth |
| --- | --- | --- | --- |
| POST | TODO | Register | No |
| POST | TODO | Login (JWT) | No |
| TODO | TODO | Sync progress by `gameId` | Yes |
| TODO | TODO | Leaderboard by `gameId` (and level) | TODO |
| TODO | TODO | Get / update level definitions | TODO |

### Error responses

TODO: the single error format and the HTTP status used for each case (§5.2.6 of the statement).

## Getting Started

### Prerequisites

TODO

### Installation

```bash
TODO
```

### Run

```bash
TODO
```

## Running Tests

```bash
TODO
```

TODO: test types (unit, integration with an in-memory database, HTTP endpoint tests including `gameId` filtering, contract tests) and how CI runs them on every pull request.

## AI Usage Documentation

See [`AI_USAGE.md`](AI_USAGE.md).

## Contributing

See [`CONTRIBUTING.md`](CONTRIBUTING.md) (Conventional Commits, branch workflow, pull request process).

## License

TODO
