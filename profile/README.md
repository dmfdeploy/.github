# dmfdeploy

**Provisioning a media workload, and what the record says**

https://github.com/user-attachments/assets/677f2278-1f5b-4bc5-9685-ae23d0a438ce


> **Independent exploratory project.** `dmfdeploy` is not affiliated with,
> endorsed by, sponsored by, or otherwise connected to the European Broadcasting
> Union (EBU). References to EBU publications, including the *Dynamic Media
> Facility* reference architecture, are for technical context and vocabulary
> alignment only.

`dmfdeploy` is an open source experiment. It studies ideas from the
[EBU](https://tech.ebu.ch/) *Dynamic Media Facility* publications on commodity
infrastructure: k3s, Ansible, NetBox, AWX, Authentik, OpenBao, and a React
operator console. A Day-0 installer container takes a blank ARM64 node toward a
small, reproducible media-operations stack. The stack covers identity, secrets
custody, a source-of-truth inventory, and a catalog of deployable media
functions.

**Proven so far** (first-party): NMOS IS-04/05 deploys and runs on commodity
ARM k3s. The platform's catalog control chain drives it end to end, from the
console through AWX and Helm to the lifecycle state in NetBox. The larger claim
is that a *stranger* can reproduce this, and v0.1 is working to show it. For
the full argument, see
[the thesis one-pager](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/THESIS.md).

**What v0.1 does not claim:** production ST 2110, PTP, or multicast
correctness, real-time media-plant behavior, multi-node high availability,
cross-site federation, or performance numbers.
Single-node is the proof surface. The rest is named future work, and this page
doesn't claim it works today.

## Start here

| You are… | Go to |
|---|---|
| **Curious or evaluating:** "What is this, and does it work?" | [THESIS](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/THESIS.md) → [dmf-init](https://github.com/dmfdeploy/dmf-init) (the Day-0 installer) |
| **A potential contributor** | [JOURNEY](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/JOURNEY.md) → [CONTRIBUTING](https://github.com/dmfdeploy/dmfdeploy/blob/main/CONTRIBUTING.md) → [Issues](https://github.com/dmfdeploy/dmfdeploy/issues) + [project board](https://github.com/orgs/dmfdeploy/projects/1) |
| **Working here with AI agents** | [WORKING-MODEL](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/WORKING-MODEL.md): how Issues, milestones, the board, Discussions, and the doc rules fit together |

**[`dmfdeploy`](https://github.com/dmfdeploy/dmfdeploy) is the front door.** It's
the umbrella repo, with the consolidated knowledge base, the decision record
(ADRs), and cross-repo coordination. The eight `dmf-*` repos are the
components. Each README says what the component does and links back to the
umbrella.

## How this org works

- **One backlog:** [umbrella Issues](https://github.com/dmfdeploy/dmfdeploy/issues).
  A milestone means an issue is scheduled. An issue opened in a component repo
  is triaged within about a week: it's closed, or linked to an umbrella issue
  where the work continues.
- **Questions and proposals:** [umbrella Discussions](https://github.com/dmfdeploy/dmfdeploy/discussions),
  for Q&A, early ideas, and the RFC that comes before a cross-cutting ADR.
- **PRs:** Conventional Commits, DCO sign-off, and rebase merges. **A PR merges
  automatically once its required reviews and checks pass**, unless it's a
  draft or carries the `hold` label.
- **Corrections:** [CORRECTIONS](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/CORRECTIONS.md)
  logs each public statement that turned out to be wrong, with the correct
  version.
- **Built with AI agents:** agents build much of the platform under the
  maintainer's direction. That's deliberate, and
  [JOURNEY](https://github.com/dmfdeploy/dmfdeploy/blob/main/docs/JOURNEY.md#working-with-agents-the-method)
  documents it as a method.

Licensed [Apache-2.0](https://github.com/dmfdeploy/dmfdeploy/blob/main/LICENSE).
