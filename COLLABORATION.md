# Collaboration Guide

## Principles
- **Open by default** – prefer issues/discussions over DMs.
- **Contracts first** – schemas drive codegen, validation, and docs.
- **Small, frequent changes** – ship small PRs with tests.
- **Users win** – prefer simplicity and safety.

## Repo Roles
- `aurenworks` (meta) • `*-studio` and `*-portal` (UI) • `*-api` (APIs) •
  `*-worker` (execution) • `*-schemas` (contracts) • `*-infra` (IaC/CI/CD) • `*-docs` (documentation)

## Branching & Releases
- Trunk-based: `main` is releasable; feature branches `feat/<name>`.
- Conventional Commits (`feat:`, `fix:`, `docs:`, `ci:` …).
- SemVer where applicable; release notes generated from commits.

## Pull Requests
- Keep scope small (~≤300 LOC).
- Include purpose, scope, screenshots (if UI), and impact (migrations/perf).
- Require green checks (tests/lint/security) and ≥1 maintainer approval.

## Testing
- Unit tests for new logic.
- Contract tests when schemas change (breaking changes require an RFC).
- E2E smoke tests per environment in `aurenworks-infra`.

## RFCs
Create `/rfcs/NNNN-short-title.md` with:
Problem, Non-goals, Proposal, Alternatives, Migration, Security/Privacy, Open questions.

## Issues & Labels
Use labels: `type:bug|feature|docs|infra`, `prio:p0|p1|p2`, `good first issue`, `help wanted`.

## Security & Privacy
No secrets in repos; use managed secrets (e.g., SOPS/Sealed Secrets).
Least privilege for tokens and cloud roles. Third-party code needs license checks.
Report vulnerabilities privately via advisories or `security@…`.

## Communication
Use GitHub Discussions for Q&A/design. Weekly triage to update roadmap.

## Contributor License
Project is **Apache-2.0**. By contributing, you agree contributions are under Apache-2.0.
Optionally sign DCO (`Signed-off-by: Name <email>`).
