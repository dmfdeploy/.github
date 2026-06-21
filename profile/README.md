# dmfdeploy

> **Independent exploratory project.** `dmfdeploy` is not affiliated with,
> endorsed by, sponsored by, or otherwise connected to the European Broadcasting
> Union (EBU). References to EBU publications, including the *Dynamic Media
> Facility* reference architecture, are for technical context and vocabulary
> alignment only.

`dmfdeploy` is an open-source experiment that explores whether ideas from the
[EBU](https://tech.ebu.ch/) *Dynamic Media Facility* publications can be studied
on commodity infrastructure: k3s, Ansible, NetBox, AWX, Authentik, OpenBao, and
a React operator console. The current prototype drives a blank ARM64 node toward
a small, reproducible media-operations stack — identity, secrets custody,
source-of-truth inventory, and a deployable media-function catalog — through a
Day-0 installer container.

**Proven so far** (first-party): NMOS IS-04/05 deploys and runs on commodity
ARM k3s, driven end-to-end through the platform's catalog control chain
(console → AWX → Helm → NetBox lifecycle state). The larger claim — that a
*stranger* can reproduce this — is what v0.1 is closing:
[the thesis one-pager](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/THESIS.md).

## Start here

| You are… | Go to |
|---|---|
| **Curious / evaluating** — "what is this and does it work?" | [THESIS](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/THESIS.md) → [dmf-init](https://github.com/dmfdeploy/dmf-init) (the Day-0 installer) |
| **A potential contributor** | [JOURNEY](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/JOURNEY.md) → [CONTRIBUTING](https://github.com/dmfdeploy/dmfdeploy/blob/main/CONTRIBUTING.md) → [Issues](https://github.com/dmfdeploy/dmfdeploy/issues) + [project board](https://github.com/orgs/dmfdeploy/projects/1) |
| **Working here with AI agents** | [WORKING-MODEL](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/WORKING-MODEL.md) — how Issues, milestones, the board, Discussions, and the doc rules fit together (enforced, not aspirational) |

**[`dmfdeploy`](https://github.com/dmfdeploy/dmfdeploy) is the front door** —
the umbrella repo with the consolidated knowledge base, decision record (ADRs),
and cross-repo coordination. The eight `dmf-*` repos are the components; each
README describes its place in this project's reading of the EBU layer vocabulary.

## How this org works

- **One backlog:** [umbrella Issues](https://github.com/dmfdeploy/dmfdeploy/issues),
  scheduled on the org board. Component-repo issues are drive-by intake only.
- **Questions / proposals:** [umbrella Discussions](https://github.com/dmfdeploy/dmfdeploy/discussions)
  (Q&A, and the RFC-before-ADR pipeline).
- **PRs:** Conventional Commits, DCO sign-off, rebase-merge; CI must be green —
  **approval lands the PR automatically**.
- Much of the platform is built by AI agents under operator orchestration — by
  design, documented as method in
  [JOURNEY](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/JOURNEY.md#working-with-agents-the-method).

Licensed [Apache-2.0](https://github.com/dmfdeploy/dmfdeploy/blob/main/LICENSE).
