---
name: potato-stack
description: Use Potato Stack (pstack/poteto) workflows for deliberate implementation, architecture, investigation, verification, and review. Use when the user asks for Potato Stack, pstack, poteto-mode, or a named pstack companion workflow.
license: MIT
---

# Potato Stack

Read [the Codex adapter](references/codex-adapter.md) before using the bundled
workflows. It maps the upstream Cursor instructions to this host and defines how
to read the reference files.

For a task using Potato Stack, read
[poteto-mode](references/pstack/skills/poteto-mode/instructions.md), including its
Harness section, and follow the matching playbook within the user's scope.
Read only the companion workflows and principle files that the task needs.

If the user names a companion workflow, read its file under
`references/pstack/skills/<name>/instructions.md`. For example:

| Request | Bundled file |
| --- | --- |
| Help choosing or using pstack | [poteto-help](references/pstack/skills/poteto-help/instructions.md) |
| Explain how code works | [how](references/pstack/skills/how/instructions.md) |
| Investigate why it was built that way | [why](references/pstack/skills/why/instructions.md) |
| Explore architecture | [architect](references/pstack/skills/architect/instructions.md) |
| Adversarial review | [interrogate](references/pstack/skills/interrogate/instructions.md) |
| Parallel attempts or coverage | [arena](references/pstack/skills/arena/instructions.md) or [swarm](references/pstack/skills/swarm/instructions.md) |

These are bundled instruction files, not separately installed skills. Read them
directly when upstream refers to `/how`, `/architect`, or another companion.
Pass delegates the adapter path and the actual workflow paths they need.

For upstream attribution, version, and packaging changes, see
[source details](references/source.md).
