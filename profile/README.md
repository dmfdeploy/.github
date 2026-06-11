# DMF Platform

An open prototype of the [EBU](https://tech.ebu.ch/) *Dynamic Media Facility*
Reference Architecture V2.0 on commodity infrastructure: k3s, Ansible, NetBox,
AWX, Authentik, OpenBao, and a React operator console. A blank ARM64 node
becomes a software-defined media facility — identity, secrets custody,
source-of-truth inventory, and a deployable media-function catalog — driven by
a Day-0 installer container.

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
README maps its place in the EBU layer model.

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
