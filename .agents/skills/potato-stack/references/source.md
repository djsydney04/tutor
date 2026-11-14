# Upstream source

This collection vendors the portable
[backnotprop/pstack mirror](https://github.com/backnotprop/pstack), pinned to
[commit 25abb38559ddbabec563646224d09eff9a250eca](https://github.com/backnotprop/pstack/tree/25abb38559ddbabec563646224d09eff9a250eca).
The mirror tracks [Cursor's pstack](https://github.com/cursor/plugins/tree/main/pstack)
and adds harness-neutral adjustments. Its original attribution and documentation
remain in [pstack/README.md](pstack/README.md),
[pstack/MIRROR.md](pstack/MIRROR.md), and [pstack/LICENSE](pstack/LICENSE).
The MIT license is copyright 2026 Lauren Tan.

## Local packaging

- `pstack/` preserves the upstream files, excluding Git internals, the
  `.cursor-plugin/` directory, and `plugin.json` manifests.
- All 61 upstream `SKILL.md` files are named `instructions.md` here: 58 primary
  workflows and three Benny automation workflows. Only this collection's root
  `SKILL.md` is a discoverable skill entrypoint.
- Local Markdown links resolving to those files and concrete bundled paths in
  inline code were mechanically updated. Generic `SKILL.md` names used when
  creating new project skills and upstream web URLs remain unchanged.
- The upstream bodies, agent templates, scripts, tests, assets, and documentation
  otherwise retain their source content. They are supporting references; their
  presence does not install plugins or activate automations.
- Trailing whitespace in the upstream README, two sponsor SVGs, and the
  automate-me instructions was normalized for the repository whitespace check.
- The root wrapper and [Codex adapter](codex-adapter.md) are local additions.
  The adapter resolves remaining bundled `SKILL.md` mentions and maps host tools,
  model selection, and authorization without rewriting the upstream workflows.

Upstream refreshes should start from the pinned source tree, repeat these
packaging transformations, inspect the change, and validate the wrapper, links,
and relevant script behavior before publishing.
