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

Editable source: [`docs/diagrams/src/`](docs/diagrams/src/)

## Generic Engine

TODO: the statement lists this section for both READMEs. Explain how the backend stays generic over `gameId` (one progress/leaderboard/level model with a per-`gameId` section) and link to the game client repository for the engine itself.

## Design Patterns

| Category | Pattern | Where (link to code) | Why |
| --- | --- | --- | --- |
| TODO | TODO | TODO | TODO |

## SOLID Principles

TODO: one subsection per principle with a real code excerpt.

## AOP

TODO: aspects implemented and the decorator/proxy strategy.

## API Documentation

TODO: Swagger / OpenAPI URL when running locally, and the path of the spec file.

| Method | Path | Description | Auth |
| --- | --- | --- | --- |
| POST | TODO | Register | No |
| POST | TODO | Login (JWT) | No |
| TODO | TODO | Sync progress by `gameId` | Yes |
| TODO | TODO | Leaderboard by `gameId` (and level) | TODO |
| TODO | TODO | Get / update level definitions | TODO |

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

## AI Usage Documentation

See [`AI_USAGE.md`](AI_USAGE.md).

## Contributing

See [`CONTRIBUTING.md`](CONTRIBUTING.md).

## License

TODO
