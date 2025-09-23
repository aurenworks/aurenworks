# Auren Works

**Auren Works** is an open, Apache 2.0–licensed citizen-developer platform powered by our dragon mascot **Auren**.
It helps teams design apps, data models, and automations—fast, safely, and at scale.

## Repository Map
- **aurenworks-studio** — No/low-code **builder UI**
- **aurenworks-portal** — Deployed app **runtime/portal**
- **aurenworks-api** — **Control-plane API** (REST/GraphQL)
- **aurenworks-worker** — **Job/flow runner** for automations
- **aurenworks-schemas** — **Shared contracts** (JSON Schema, OpenAPI, GraphQL, Protobuf, events)
- **aurenworks-docs** — **Docs site** (guides, tutorials, API reference)
- **aurenworks-infra** — **IaC/CI/CD** (Terraform, Helm, K8s)
- **aurenworks** — **Meta repo**: roadmap, RFCs, governance, brand

## Vision
Empower anyone to turn ideas into running software through thoughtful defaults, strong contracts, and industrial-grade operations.

## Architecture at a Glance
Studio ↔ API (models, flows, assets) • Schemas drive codegen/validation •
Worker executes flows/events • Portal serves end-user experiences with RBAC •
Infra provides environments/observability/delivery • Docs tie it together.

## Getting Started
This repo tracks cross-cutting docs and issues. Build/run instructions live in each service repo.

- Central planning here; service-specific bugs live in their repo and link back.
- Propose major changes via RFCs in `rfcs/`.

## Roadmap
See [`/roadmap`](./roadmap). We use GitHub Projects to track epics across repos.

## Contributing
Please read **[COLLABORATION.md](./COLLABORATION.md)** before contributing.

## Security
Report vulnerabilities privately via GitHub Security Advisories or `security@aurenworks.example`.

## License
Licensed under the **Apache License, Version 2.0**. See [`LICENSE`](./LICENSE).
