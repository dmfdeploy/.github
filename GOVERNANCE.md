# Governance

*Org-wide default; one page on purpose.*

- **Canonical governance model:** **ADR-0041 — DMF Release and Contribution
  Model**, in the umbrella repo
  ([docs/decisions/](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/decisions/INDEX.md)).
  Cross-cutting decisions are recorded as ADRs there; substantial ones start
  as RFC threads in
  [Discussions](https://github.com/dmfdeploy/dmfdeploy/discussions).
- **Maintainers:** the `@dmfdeploy/maintainers` team (CODEOWNERS in every
  repo). A maintainer review is required to merge; there is no bypass on
  `main`.
- **Change process:** GitHub PRs only — Conventional Commits, DCO sign-off
  (`git commit -s`), rebase-merge, linear history, required CI green.
  Approval auto-lands the PR (`hold` label defers).
- **Day-to-day working model** (issues, milestones, project board,
  documentation rules):
  [docs/WORKING-MODEL.md](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/WORKING-MODEL.md).
- **License:** Apache-2.0 across the org; contributions are accepted under it
  via the DCO (no CLA).
