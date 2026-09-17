# Repository Architecture

## Architecture Overview

The repository follows a monorepo-style structure that separates
the client, server, documentation and testing concerns.

## Architecture Tree

```text
accessibility-baseline-audit/
│
├── client/
│ └── README.md
│
├── server/
│ └── README.md
│
├── docs/
│ ├── audit-report.md
│ ├── architecture.md
│ └── screenshots/
│
├── tests/
│ └── README.md
│
├── README.md
└── .gitignore

Components

Client
Reserved for the frontend application.

Server
Reserved for backend services and APIs.

Documentation
Contains the accessibility audit, architecture documentation and supporting evidence screenshots.

Tests
Reserved for automated and manual testing resources.

Maintainability
Separating application layers and documentation makes the repository easier to extend into a complete full-stack project.
