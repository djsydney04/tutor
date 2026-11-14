# Shared skills catalog

This library contains **38 shared skills** and **14 project packages**, plus **58 Potato Stack workflows and principles** bundled behind one entrypoint. The three Benny automation references are included separately and remain inactive.

Agents choose relevant skills automatically using [skill-routing.md](guidance/skill-routing.md). You can also ask explicitly, for example `Use $persona-designer`, `Use $ponytail`, `Use $test-audit`, or `Use $cloudflare`. Each table links to the actual instructions.

Use the `skills/` collection and `guidance/` beside this catalog. In a repository
initialized from this library, these files live together under `.agents/` and
the root `AGENTS.md` points here. Read each selected skill's `SKILL.md` before
following its workflow. The repository copy is a one-time snapshot that can be
edited independently; it does not follow changes in the shared source.

When accessing the shared library through a symlink, resolve the catalog's
canonical location before following relative links. Local installation and
workspace shortcuts are documented in the source repository's README.

**Modes:** “Report” means no source edits; checks can still create disposable runtime output. “Plan” produces recommendations without implementation. “Edit” can change files within the requested task. Reading a skill does not authorize deployment, external messages, account changes, or publication. The [routing guide](https://github.com/djsydney04/agent-skills/blob/main/guidance/skill-routing.md), project instructions, and existing user authorization determine the allowed work.

## Shared personas

Choose the role that owns the requested outcome, then load only the matching
resources from its fleet. These four skills add reusable judgment to the 34
existing shared skills. They do not require optional plugins or activate every
Potato Stack workflow. Follow an already selected Ponytail or specialist route
once rather than repeating the same pass through each router.

| Skill | What it does | When to use it | Mode |
| --- | --- | --- | --- |
| [persona-designer](skills/persona-designer/SKILL.md) | Connects user needs, journeys, information architecture, interaction, visual hierarchy, accessibility, and evaluation. | Product design, UI/UX, a designer role, prototypes, or decisions about a product experience. | Research, critique, concept, or implementation as requested; checks the actual interface when available. |
| [persona-engineer](skills/persona-engineer/SKILL.md) | Combines Ponytail's smallest complete change with suitable data models, boundaries, root-cause investigation, and risk-based verification. | Everyday implementation and technical decisions, or an engineer role coordinating these concerns. | The requested implementation, investigation, review, or planning mode; chooses one appropriate specialist workflow. |
| [persona-marketer](skills/persona-marketer/SKILL.md) | Connects audience evidence, positioning, credible messaging, channel choices, and experiments to business outcomes. | A marketer role, value propositions, marketing copy, campaign strategy, or experiment design. | Research, strategy, draft, or scoped execution; sending, publishing, and campaign spending need existing or task-specific authorization. |
| [persona-business-ops](skills/persona-business-ops/SKILL.md) | Clarifies workflows, ownership, capacity, status, budgets, operating decisions, and their supporting evidence. | A business ops role, operating plans, process improvements, resource decisions, or budget and capacity analysis. | Analysis, plan, document, or scoped execution; a recommendation does not authorize changing live records or spending. |

## Visual design and reference study

Use these focused workflows through Designer or directly. They preserve the
target's brand, platform conventions, behavior, and requested mode. A familiar
component or a particular color is not automatically a design defect.

| Skill | What it does | When to use it | Mode |
| --- | --- | --- | --- |
| [design-taste](skills/design-taste/SKILL.md) | Chooses and carries through visual direction using product context, typography, hierarchy, density, imagery, and reference study. | Art direction, visual polish, taste, or applying the user's design references to a landing page or product interface. | Critique, plan, or implementation as requested; verifies the actual artifact when available. |
| [deslop-ui](skills/deslop-ui/SKILL.md) | Finds interchangeable visual and content patterns and replaces their cause with purposeful design decisions. | Deslop/unvibe requests, repetitive landing pages, generic UI, or a focused visual finish. | Reviews report findings; fixes and builds make scoped changes under existing authorization. |

The [design reference index](skills/design-taste/references/design-index.md) is
the single home for the user's seven selected sites. It separates confirmed
preferences from provisional style interpretations and records inspection limits.
The [tells checklist](skills/deslop-ui/references/tells.md) and
[source notes](skills/design-taste/references/sources.md) support the workflows
without importing or installing an external skill bundle.

## Project packages

These 14 packages live under `projects/<id>/skills/`, separately from shared
skills. Each applies to the named repository and its linked worktrees, or an
explicit request about that project. Read the target checkout's `AGENTS.md` and
module instructions, and resolve a package's `SKILL.md` through symlinks before
following its library-relative references.

Global and workspace shared-skill discovery expose only the 38 shared skills.
A project checkout or worktree exposes its own matching project package. Only
the central library's primary checkout exposes every project package for discovery
and maintenance. Their central availability does not make unrelated project
guidance applicable, and existing project-local skills remain intact.

| Project skill | What it does | When to use it |
| --- | --- | --- |
| [project-agent-sandbox](https://github.com/djsydney04/agent-skills/blob/main/projects/agent-sandbox/skills/project-agent-sandbox/SKILL.md) | Guides the Rust sandbox CLI, container configuration, and gateway boundaries while preserving explicit host capabilities and isolation. | Work in Agent Sandbox or its worktrees, or an explicit request about its CLI, containers, or gateway behavior. |
| [project-agent-skills](https://github.com/djsydney04/agent-skills/blob/main/projects/agent-skills/skills/project-agent-skills/SKILL.md) | Maintains shared workflows, routing, publishing, project packages, and workspace installation while preserving clean-main updates and scoped discovery. | Work in this library or its worktrees, or an explicit request about its skills, installer, updater, or discovery. |
| [project-cloud-agents](https://github.com/djsydney04/agent-skills/blob/main/projects/cloud-agents/skills/project-cloud-agents/SKILL.md) | Guides Rust/Axum services, the Electron desktop, container packaging, and relevant deployment integrations, including shared contracts and durable task state. | Work in Cloud Agents or its worktrees, or an explicit request about its service, desktop, packaging, or deployment integration. |
| [project-codex-review](https://github.com/djsydney04/agent-skills/blob/main/projects/codex-review/skills/project-codex-review/SKILL.md) | Guides Rust review logic, Python service integration, and GitHub worker behavior, with representative benign and adversarial review inputs. | Work in Codex Review or its worktrees, or an explicit request about its review engine, Python service, or worker. |
| [project-greenroom-monorepo](https://github.com/djsydney04/agent-skills/blob/main/projects/greenroom-monorepo/skills/project-greenroom-monorepo/SKILL.md) | Guides native Swift interfaces, Next.js workspaces, supporting services, and product design using the relevant platform and Green Room brand conventions. | Work in Green Room or its worktrees, or an explicit request about its clients, services, or product experiences. |
| [project-init](https://github.com/djsydney04/agent-skills/blob/main/projects/init/skills/project-init/SKILL.md) | Guides the Rust control plane, Tauri desktop, and JavaScript/Rust SDKs while keeping interface, lifecycle, version, and generated-binding contracts aligned. | Work in Init or its worktrees, or an explicit request about its control plane, desktop, or SDKs. |
| [project-llm-proj](https://github.com/djsydney04/agent-skills/blob/main/projects/llm-proj/skills/project-llm-proj/SKILL.md) | Guides the Rust scheduling agent, provider clients, evaluation tools, and optional TUI; separates validated constraints and offline checks from live-model results. | Work in LLM Project or its worktrees, or an explicit request about its scheduling, provider, evaluation, or TUI behavior. |
| [project-operating-systems](https://github.com/djsydney04/agent-skills/blob/main/projects/operating-systems/skills/project-operating-systems/SKILL.md) | Guides C/C++ assignments using each assignment's requirements, makefiles, interfaces, concurrency rules, cleanup, and tests. | Work in Operating Systems or its worktrees, or an explicit request about an assignment in that repository. |
| [project-payment-mesh](https://github.com/djsydney04/agent-skills/blob/main/projects/payment-mesh/skills/project-payment-mesh/SKILL.md) | Guides Rust components, native iOS/FFI contracts, and payment or cryptographic integrations, preserving money, retry, signing, and transaction-state contracts. | Work in Payment Mesh or its worktrees, or an explicit request about its components and integrations. |
| [project-prism-wiki](https://github.com/djsydney04/agent-skills/blob/main/projects/prism-wiki/skills/project-prism-wiki/SKILL.md) | Guides documentation/source synchronization and verification against the companion Prism checkout, preserving generated/manual boundaries and API revision alignment. | Work in Prism Wiki or its worktrees, or an explicit request about its source entries, generated docs, update tools, or verification. |
| [project-repo-maintainer](https://github.com/djsydney04/agent-skills/blob/main/projects/repo-maintainer/skills/project-repo-maintainer/SKILL.md) | Guides the Rust maintenance CLI, documentation inputs, target selection, repository writes, and verification using disposable repositories. | Work in Repo Maintainer or its worktrees, or an explicit request about its maintenance commands and repository changes. |
| [project-rust-sdks](https://github.com/djsydney04/agent-skills/blob/main/projects/rust-sdks/skills/project-rust-sdks/SKILL.md) | Guides Rust SDKs / Prism shared provider contracts and coordinated crate changes, including streaming, errors, feature flags, and representative callers. | Work in Rust SDKs / Prism or its worktrees, or an explicit request about its core contracts, provider crates, or SDK changes. |
| [project-software-factory](https://github.com/djsydney04/agent-skills/blob/main/projects/software-factory/skills/project-software-factory/SKILL.md) | Guides product/design documents, design-skills, and implementation planning, checking actual files before treating planned architecture as implemented behavior. | Work in Software Factory or its worktrees, or an explicit request about its product documents, design-skills, or implementation plans. |
| [project-software-factory-prototype](https://github.com/djsydney04/agent-skills/blob/main/projects/software-factory-prototype/skills/project-software-factory-prototype/SKILL.md) | Guides the React/Vite desktop preview and interaction experiments, verifying the running frontend and distinguishing simulated from live backend operations. | Work in Software Factory Prototype or its worktrees, or an explicit request about its desktop preview and interaction experiments. |

Project packages retain the requested review, planning, or implementation mode.
They grant no extra account, publication, deployment, spending, deletion, or
messaging authority. Keep Software Factory and Software Factory Prototype
distinct even when their remote names overlap.

## Everyday development and reviews

| Skill | What it does | When to use it | Mode |
| --- | --- | --- | --- |
| [ponytail](skills/ponytail/SKILL.md) | Finishes the task with the smallest complete change, reusing existing code and avoiding unnecessary dependencies or abstractions. | Everyday coding, bug fixes, refactoring, and dependency choices; `lite`, `full`, and `ultra` adjust how strongly it challenges extra scope. | Edit within the task; the selected style stays active until changed. |
| [ponytail-review](skills/ponytail-review/SKILL.md) | Reviews a change and its connected code for concrete bugs, security risks, load problems, missing protection, slowness, and unnecessary complexity. | A diff, branch, pull request, or changed files need review. | Report; does not apply fixes. |
| [ponytail-audit](skills/ponytail-audit/SKILL.md) | Maps the requested repository or area and ranks actionable correctness, security, scaling, testing, performance, and simplification findings. | You request an audit of a repository, package, or folder. | Report; does not change code. |
| [ponytail-debt](skills/ponytail-debt/SKILL.md) | Collects deliberate `shortcut:` and older `ponytail:` comments into a ledger of limits and triggers for revisiting them. | Find what was intentionally deferred or which shortcuts lack an upgrade trigger. | Report; saves a ledger only when requested. |
| [ponytail-gain](skills/ponytail-gain/SKILL.md) | Shows Ponytail's published upstream benchmark results and explains their limits. | Understand the benchmark's measured code, token, cost, and time differences. | Display only; these are **not measurements of your project**. |
| [ponytail-help](skills/ponytail-help/SKILL.md) | Explains Ponytail levels, related skills, activation, and host-specific limitations. | Choose a level or learn how to use the Ponytail collection. | Display only; does not change modes or settings. |
| [potato-stack](skills/potato-stack/SKILL.md) | Coordinates deliberate implementation, architecture, investigation, verification, and review through the bundled workflows below. | Substantial changes, difficult investigations, migrations, architecture decisions, or an explicit Potato Stack request. | Depends on the selected workflow; read the [Codex adapter](skills/potato-stack/references/codex-adapter.md) first. |

Ponytail supplies the simplicity preference. Potato Stack adds a suitable workflow when the task needs more structure. A small change does not need every workflow or an extra review pass.

## Testing and shared-library maintenance

| Skill | What it does | When to use it | Mode |
| --- | --- | --- | --- |
| [test-principles](skills/test-principles/SKILL.md) | Defines a valuable test through an observable promise, a plausible failure, a suitable boundary, and an independent expected result. | Discuss test quality or begin any of the testing workflows below. | Guidance; does not start an audit by itself. |
| [test-audit](skills/test-audit/SKILL.md) | Checks whether existing tests detect meaningful failures, miss consequential risks, duplicate protection, or fail unreliably. | Assess the tests for a feature, change, or requested suite. | Report; leaves source, tests, fixtures, and configuration unchanged. |
| [test-plan](skills/test-plan/SKILL.md) | Produces a minimal prioritized plan mapping risks to test boundaries, setup, and observable assertions. | Decide which tests are needed before implementing them. | Plan; no tests, application edits, dependency installation, or harness redesign. |
| [test-write](skills/test-write/SKILL.md) | Adds or improves focused tests that expose a named behavior failure using the project's existing conventions. | Implement a useful regression test or improve weak protection for an identified behavior. | Edit tests within scope and run appropriate checks. |
| [test-stabilize](skills/test-stabilize/SKILL.md) | Diagnoses an intermittent failure, fixes its supported cause, and checks stability under the relevant conditions. | A test is flaky because of timing, shared state, cleanup, uncontrolled inputs, or environment behavior. | Edit the relevant test or harness; product fixes require scope covering that cause. |
| [skill-publish](skills/skill-publish/SKILL.md) | Authors or improves a shared skill, validates it, commits the selected skill, pushes it, and refreshes discovery links. | Save a reusable workflow in this shared repository. | Edit and scoped publication when requested here; honors draft and local-only requests. |

## Cloudflare

These 19 skills come from Cloudflare's official skills collection. They retrieve current documentation and inspect the project's installed versions before giving exact API or command guidance. Importing them does not install CLIs, connect an account, provision resources, deploy applications, or run their bundled scripts. See [source and license details](skills/cloudflare/references/source.md).

| Skill | What it does | When to use it | Scope to expect |
| --- | --- | --- | --- |
| [cloudflare](skills/cloudflare/SKILL.md) | Starts from the goal, selects suitable Cloudflare products, and routes to their focused skills or documentation. | Architecture, platform choices, or a Cloudflare task without a known product. | Discovery and planning first; implementation follows the requested task. |
| [cf-cli](skills/cf-cli/SKILL.md) | Finds and verifies commands for Cloudflare's `cf` CLI, including account profiles, Workers projects, and API resources. | A new project uses `cf`, or you need Cloudflare API/resource commands and CLI selection help. | CLI guidance and requested operations; distinguishes previews from commands that change resources. |
| [wrangler](skills/wrangler/SKILL.md) | Uses the project's Wrangler version and configuration for development, builds, previews, deployment, and resource management. | An existing project has Wrangler configuration or you explicitly request Wrangler. | Requested local or remote operations; checks the target account, environment, and resource. |
| [workers-best-practices](skills/workers-best-practices/SKILL.md) | Applies Workers guidance for runtime behavior, streaming, promise lifetime, bindings, configuration, observability, and security. | Write, review, or configure Workers code. | Edit for implementation; report only for a review. |
| [workers-profiling](skills/workers-profiling/SKILL.md) | Captures and examines CPU or heap profiles to identify expensive functions and allocations in deployed Workers or Durable Objects. | Investigate CPU cost, latency, memory pressure, or growth using deployed-code evidence. | Profiling and recommendations; identifies the actual deployment before a capture. |
| [agents-sdk](skills/agents-sdk/SKILL.md) | Builds and diagnoses applications using Cloudflare's Agents SDK, including state, RPC, scheduling, WebSockets, chat, and workflows. | Build, debug, or review an `agents` package application. | Code and configuration within the requested build or review. |
| [durable-objects](skills/durable-objects/SKILL.md) | Designs and checks persistent state, coordination, storage, RPC, alarms, WebSockets, and Durable Object tests. | Stateful rooms, per-entity storage, strongly consistent coordination, or Durable Object debugging. | Implementation or review; includes bindings, migrations, and concurrency considerations. |
| [gateway-workers](skills/gateway-workers/SKILL.md) | Implements Workers called by Gateway HTTP Forward policies, including the middleware entrypoint, identity context, and request continuation. | Transform, inspect, or respond to permitted Gateway traffic through a Worker. | Code and scoped Gateway-path validation; policy rollout stays within the task. |
| [cloudflare-one](skills/cloudflare-one/SKILL.md) | Designs, inspects, and troubleshoots Zero Trust/SASE access, traffic policies, device posture, tunnels, identity, and networking. | Cloudflare Access, Gateway, WARP, Tunnel, WAN, DLP, CASB, or related security work. | Assessment or requested configuration; uses scoped pilots and rollback planning where relevant. |
| [cloudflare-one-migrations](skills/cloudflare-one-migrations/SKILL.md) | Maps an existing VPN, SWG, or SASE setup to Cloudflare One and records parity gaps, dependencies, and rollout gates. | Plan a move from Zscaler, Palo Alto, a legacy VPN, or another network-security stack. | Migration assessment and plan first; executing a cutover is a separate scoped action. |
| [cloudflare-email-service](skills/cloudflare-email-service/SKILL.md) | Implements and diagnoses transactional email sending, incoming email routing, provider bindings, and delivery prerequisites. | Add or repair Cloudflare Email Sending or Email Routing integration. | Code/configuration work; importing it grants no permission to send messages. |
| [basin](skills/basin/SKILL.md) | Guides event ingestion and transformation, R2 Iceberg catalogs, and analytical SQL through the Basin product family. | Data pipelines, catalogs, and SQL analytics, including requests using earlier Data Platform names. | Planning, code, or requested data-resource operations; verifies evolving names and commands. |
| [k2](skills/k2/SKILL.md) | Guides durable event streams, producers, subscriptions, retention, inputs, acknowledgements, and consumer behavior. | Decouple event producers and consumers using K2 or K2 Streams. | Integration/configuration within scope; retrieves current availability and API documentation. |
| [nextjs-on-cloudflare](skills/nextjs-on-cloudflare/SKILL.md) | Routes new Next.js projects and requested Workers migrations through vinext's upstream setup and compatibility guidance. | Start or move a Next.js application on Cloudflare, or evaluate vinext versus an existing OpenNext setup. | Requested setup/migration; preserves existing setups during unrelated maintenance. |
| [sandbox-stable](skills/sandbox-stable/SKILL.md) | Uses the stable Sandbox package and matching container image for isolated execution, files, processes, terminals, and lifecycle work. | Maintain an application on stable `@cloudflare/sandbox`, including stable API cleanup. | Code/configuration work; does not silently move the application to preview. |
| [sandbox-next](skills/sandbox-next/SKILL.md) | Uses Sandbox SDK 1.0 preview contracts and matching preview images, including process handles and explicit command observation. | Build or maintain an app using `@cloudflare/sandbox@next`. | Preview-line work; routes stable applications to the stable or migration skill. |
| [sandbox-migrate-to-next](skills/sandbox-migrate-to-next/SKILL.md) | Audits and ports stable Sandbox code, package versions, and container images to the preview's changed execution contracts. | You request a stable-to-preview migration. | Migration edits and validation; production cutover is not implied by routine maintenance. |
| [turnstile-spin](skills/turnstile-spin/SKILL.md) | Wires Turnstile widgets and canonical backend Siteverify checks into an existing application, including repair or CAPTCHA migration. | Protect a form, endpoint, signup, download, or other user action against bots. | Frontend/backend edits and requested widget configuration; keeps secrets outside chat and source control. |
| [web-perf](skills/web-perf/SKILL.md) | Uses available browser traces, network evidence, and source inspection to assess loading, interaction performance, and Core Web Vitals. | Audit slow pages, diagnose a Lighthouse result, or perform requested performance improvements. | Report for an audit; edit only when optimization work is requested. |

The imported guidance distinguishes the `cf` and Wrangler project setups, stable and preview Sandbox packages, and migration versus maintenance. Agents inspect the actual project before selecting those branches. Optional integrations and scripts still need their normal tools, credentials, and relevant authorization.

## Potato Stack: understanding and communication

The following are **bundled reference workflows, not separately installed global skills**. Ask for `Use $potato-stack how to explain this subsystem`, or `Use $potato-stack interrogate to review this change`. Agents can select them automatically too. The adapter maps upstream commands, delegation, and host-specific tools to the current environment; it does not activate Cursor settings or automation.

| Workflow | What it does and when to use it | Mode |
| --- | --- | --- |
| [poteto-help](skills/potato-stack/references/pstack/skills/poteto-help/instructions.md) | Explains the collection and helps choose a workflow, playbook, or principle for the task. | Guidance. |
| [how](skills/potato-stack/references/pstack/skills/how/instructions.md) | Traces code ownership, architecture, and runtime flow to explain how a subsystem works or where a change belongs. | Report; no code edits. |
| [why](skills/potato-stack/references/pstack/skills/why/instructions.md) | Investigates the reasons behind a design using source history and relevant connected evidence, separating findings from guesses. | Investigation; no source edits or external posts. |
| [teach](skills/potato-stack/references/pstack/skills/teach/instructions.md) | Combines `how` and `why` into a plain explanation suited to the reader's question and experience. | Explanation; no implementation. |
| [recall](skills/potato-stack/references/pstack/skills/recall/instructions.md) | Reconstructs the current state of a named workstream from relevant chat history, live branches/PRs, and shared evidence. | Scoped investigation and status brief. |
| [ketchup](skills/potato-stack/references/pstack/skills/ketchup/instructions.md) | Catches you up on changes since your previous message and lists decisions that still need your input. | Read-only status report; does not start jobs or change code. |
| [ketchup-video](skills/potato-stack/references/pstack/skills/ketchup-video/instructions.md) | Presents the same catch-up as a short subtitled slide video built from actual evidence. | Writes a video outside the repo; otherwise read-only. |
| [bro](skills/potato-stack/references/pstack/skills/bro/instructions.md) | Restates the agent's previous reply in shorter, ordinary language without jargon. | Reply only. |
| [in-your-own-words](skills/potato-stack/references/pstack/skills/in-your-own-words/instructions.md) | Restates the user's goals and underlying problem to check understanding. | Reply only. |
| [sharpen](skills/potato-stack/references/pstack/skills/sharpen/instructions.md) | Rewrites a task to seek deeper evidence and stronger methods without increasing its scope or deciding the user's choices. | Prompt proposal only. |
| [technical-writing](skills/potato-stack/references/pstack/skills/technical-writing/instructions.md) | Shapes documentation, RFCs, README files, PR text, and commit messages around the reader's job and clear technical language. | Draft, edit, or review prose as requested. |
| [unslop](skills/potato-stack/references/pstack/skills/unslop/instructions.md) | Removes stock AI phrasing, vague claims, filler, jargon, and repetitive writing while preserving meaning. | Prose edit or suggested rewrite. |

## Potato Stack: planning, implementation, and coordination

| Workflow | What it does and when to use it | Mode |
| --- | --- | --- |
| [poteto-mode](skills/potato-stack/references/pstack/skills/poteto-mode/instructions.md) | Supplies the main deliberate-work style, principles, delegation rules, verification expectations, and matching playbooks. | Scope follows the requested task and selected playbook. |
| [architect](skills/potato-stack/references/pstack/skills/architect/instructions.md) | Grounds the existing system, compares alternative type/module sketches, and guides implementation against the chosen shape. | Planning, then implementation when in scope; can stop at a sketch. |
| [arena](skills/potato-stack/references/pstack/skills/arena/instructions.md) | Creates independent candidates, evaluates them against one rubric, combines their strongest parts, and verifies the result. | Produces the requested artifact; isolates concurrent writers. |
| [swarm](skills/potato-stack/references/pstack/skills/swarm/instructions.md) | Splits coverage across parallel workers or races attempts, then drains them into one checked report or artifact. | Each worker receives its own explicit scope and side effects. |
| [figure-it-out](skills/potato-stack/references/pstack/skills/figure-it-out/instructions.md) | Designs an auditable phased workflow for a migration or ambitious task when no narrower playbook fits. | Framing and planning, followed by scoped execution and verification. |
| [correct](skills/potato-stack/references/pstack/skills/correct/instructions.md) | Turns recurring agent mistakes into structural prevention, preferring architecture, types, lint, or tests over repeated reminders. | Edits the relevant structure/checks and proves they catch the past mistake. |
| [setup-pstack](skills/potato-stack/references/pstack/skills/setup-pstack/instructions.md) | Configures per-role model choices and reasoning budgets using models actually available in the host. | Settings change only when setup is requested; normal use inherits the parent model. |
| [automate-me](skills/potato-stack/references/pstack/skills/automate-me/instructions.md) | Turns relevant working preferences and repeated conventions into a personal `-mode` skill. | Creates or revises a skill; no automation is enabled merely by doing so. |
| [reflect](skills/potato-stack/references/pstack/skills/reflect/instructions.md) | Reviews the active conversation for durable lessons and applies useful improvements to existing skills. | Scoped skill edits; shared publication follows `skill-publish`. |
| [show-me-your-work](skills/potato-stack/references/pstack/skills/show-me-your-work/instructions.md) | Keeps a compact TSV decision log with reasons, evidence, and outcomes for long or unattended work. | Writes a local log; commits it only within the delivery scope. |
| [make-bot-ui](skills/potato-stack/references/pstack/skills/make-bot-ui/instructions.md) | Describes a local UI that wakes a webhook bot, keeps the sender key server-side, and can be exposed on Tailscale. | Builds/configures integrations only when requested and supported; upstream bot tools are host-specific. |

## Potato Stack: verification and focused checks

| Workflow | What it does and when to use it | Mode |
| --- | --- | --- |
| [benchmark-checklist](skills/potato-stack/references/pstack/skills/benchmark-checklist/instructions.md) | Checks bottlenecks, tuning, errors, noise, repeatability, and relevance before trusting a measured performance claim. | Measurement and evidence review; not an automatic optimization pass. |
| [blast-radius](skills/potato-stack/references/pstack/skills/blast-radius/instructions.md) | Finds effects beyond a small diff and runs real code to prove the assumptions that make the change safe. | Investigation with focused executable probes; no implicit fixes. |
| [interrogate](skills/potato-stack/references/pstack/skills/interrogate/instructions.md) | Runs independent adversarial reviews and retains only findings reproduced against real code or a relevant prototype. | Report; repros stay in isolated worktrees and fixes are not applied. |
| [no-comments](skills/potato-stack/references/pstack/skills/no-comments/instructions.md) | Audits scoped comments, removes accepted noise, and addresses in-scope code problems hidden behind explanations or suppressions. | **Edits comments and potentially code**; this is not a read-only review. |
| [create-verification-skill](skills/potato-stack/references/pstack/skills/create-verification-skill/instructions.md) | Creates a project-local skill and feature map that launch and drive the actual app, CLI, or service with repeatable evidence. | Writes the verification skill/harness and proves its instructions work. |
| [maintain-verification-skill](skills/potato-stack/references/pstack/skills/maintain-verification-skill/instructions.md) | Reconciles an existing verification skill and feature map with source and live behavior, distinguishing documentation drift from product bugs. | Edits only the verification skill's directory; reports product defects. |
| [create-formal-verification-skill](skills/potato-stack/references/pstack/skills/create-formal-verification-skill/instructions.md) | Chooses an important hard-to-test property, verifies it with a fitting formal tool, and leaves a reusable project-local verification skill. | Creates verification artifacts; any proof is limited by its model, assumptions, and bounds. |
| [maintain-formal-verification-skill](skills/potato-stack/references/pstack/skills/maintain-formal-verification-skill/instructions.md) | Checks changes since the last verified revision, updates stale models/harnesses, and separates verification drift from actual bugs. | Edits verification only; does not weaken properties or fix product code without that scope. |
| [statechart](skills/potato-stack/references/pstack/skills/statechart/instructions.md) | Checks a TLA+ model and renders a Mermaid statechart with shortest paths to states that violate a rule. | Produces scratch models and report artifacts; tools may need a TypeScript runtime, Java/TLC, and network access. |
| [tdd](skills/potato-stack/references/pstack/skills/tdd/instructions.md) | Writes a focused failing regression test before a small bug fix when explicitly requested or when a cheap local test path is clear. | Edits tests and implementation; uses other verification when a new test is impractical. |
| [typescript-best-practices](skills/potato-stack/references/pstack/skills/typescript-best-practices/instructions.md) | Applies domain types, validated boundaries, exhaustive variants, and safe narrowing when reading or editing TypeScript. | Guidance for the requested code change or review. |

The PR, deployment, and automation steps in upstream playbooks apply only when that delivery is authorized. Bundled scripts are reviewed before use; a script described as read-only may still fetch remote state or create output.

## Potato Stack: the 24 principles

Principles are focused decision rules, not additional jobs to run. An agent loads the ones that fit its current assignment and applies them within the existing scope.

| Principle | What it means and when it helps |
| --- | --- |
| [attack-the-premise](skills/potato-stack/references/pstack/skills/principle-attack-the-premise/instructions.md) | When repeated fixes fail the same check, name and test their shared assumption before trying another fix based on it. |
| [boundary-discipline](skills/potato-stack/references/pstack/skills/principle-boundary-discipline/instructions.md) | Validate external inputs at real system boundaries and keep internal business logic separate from framework wiring. |
| [build-the-lever](skills/potato-stack/references/pstack/skills/principle-build-the-lever/instructions.md) | For substantial work, create the smallest rerunnable script, codemod, generator, or shared recipe that performs or verifies it. |
| [encode-lessons-in-structure](skills/potato-stack/references/pstack/skills/principle-encode-lessons-in-structure/instructions.md) | Replace repeated reminders with enforceable types, lint, metadata, runtime checks, or scripts when the rule can be encoded. |
| [exhaust-the-design-space](skills/potato-stack/references/pstack/skills/principle-exhaust-the-design-space/instructions.md) | Compare a few concrete alternatives before committing to an unfamiliar architecture or an interaction whose quality depends on feel. |
| [experience-first](skills/potato-stack/references/pstack/skills/principle-experience-first/instructions.md) | Choose a polished core experience over extra controls or implementation convenience, including the experience of API users and maintainers. |
| [explain-the-number](skills/potato-stack/references/pstack/skills/principle-explain-the-number/instructions.md) | Define the decision a measurement should inform, identify its limiting resource, and rule out noise, skipped work, or errors before reporting it. |
| [fix-root-causes](skills/potato-stack/references/pstack/skills/principle-fix-root-causes/instructions.md) | Trace a reproduced symptom to the first wrong system decision and fix the fault rather than hiding its consequences. |
| [foundational-thinking](skills/potato-stack/references/pstack/skills/principle-foundational-thinking/instructions.md) | Choose sound data structures, ownership, and useful scaffolding early so later implementation is straightforward. |
| [guard-the-context-window](skills/potato-stack/references/pstack/skills/principle-guard-the-context-window/instructions.md) | Bound large phases and route bulk reading to useful delegates so the coordinator retains decisions and evidence rather than raw output. |
| [laziness-protocol](skills/potato-stack/references/pstack/skills/principle-laziness-protocol/instructions.md) | Prefer the smallest complete diff, consolidate repeated decisions, and avoid layers or boilerplate without a present need. |
| [make-operations-idempotent](skills/potato-stack/references/pstack/skills/principle-make-operations-idempotent/instructions.md) | Design commands and lifecycle steps to reach the same correct state after retries, duplicate execution, or a partial prior run. |
| [migrate-callers-then-delete-legacy-apis](skills/potato-stack/references/pstack/skills/principle-migrate-callers-then-delete-legacy-apis/instructions.md) | Move internal callers to the new API and remove the old path together when external compatibility is not required. |
| [minimize-reader-load](skills/potato-stack/references/pstack/skills/principle-minimize-reader-load/instructions.md) | Reduce needless indirection and hidden mutable state so a reader can trace where values come from and what changes them. |
| [model-the-domain](skills/potato-stack/references/pstack/skills/principle-model-the-domain/instructions.md) | Use a data model, state machine, registry, or other fitting structure when scattered branches and synchronized flags encode the same domain rule. |
| [never-block-on-the-human](skills/potato-stack/references/pstack/skills/principle-never-block-on-the-human/instructions.md) | Continue authorized, reversible work with reasonable decisions while keeping genuine user choices and consequential actions within their authority. |
| [outcome-oriented-execution](skills/potato-stack/references/pstack/skills/principle-outcome-oriented-execution/instructions.md) | During a planned migration, converge on the verified target design rather than accumulating temporary compatibility code to keep every intermediate step smooth. |
| [prove-it-works](skills/potato-stack/references/pstack/skills/principle-prove-it-works/instructions.md) | Check the actual artifact or runtime behavior before declaring completion, preferably with a repeatable direct check. |
| [redesign-from-first-principles](skills/potato-stack/references/pstack/skills/principle-redesign-from-first-principles/instructions.md) | Ask what the design would look like if the new requirement had existed from the start, then deliver that coherent change incrementally. |
| [separate-before-serializing-shared-state](skills/potato-stack/references/pstack/skills/principle-separate-before-serializing-shared-state/instructions.md) | Give concurrent writers independent owned state where possible; use structural serialization only when a shared write target is required. |
| [sequence-verifiable-units](skills/potato-stack/references/pstack/skills/principle-sequence-verifiable-units/instructions.md) | Break multi-step work into small units with an observable check after each, and order the delivery so reviewers can follow the proof. |
| [subtract-before-you-add](skills/potato-stack/references/pstack/skills/principle-subtract-before-you-add/instructions.md) | Remove dead code and redundant structure before adding or polishing a new capability. |
| [test-behavior-not-implementation](skills/potato-stack/references/pstack/skills/principle-test-behavior-not-implementation/instructions.md) | Keep tests that fail when an observable promise breaks and remain valid when only internal structure changes. |
| [type-system-discipline](skills/potato-stack/references/pstack/skills/principle-type-system-discipline/instructions.md) | Make invalid states and mixed-up semantic values hard to express, parse external data once, and derive types from authoritative schemas. |

## Dormant Benny automation references

These files document an optional upstream automation pack. They are **not global skills, scheduled jobs, or connected bots**. They need explicit setup, supported host capabilities, external configuration, and authorized integrations before any operational use.

| Reference | What it does when separately configured |
| --- | --- |
| [setup-benny](skills/potato-stack/references/pstack/automations/benny/skills/setup-benny/instructions.md) | Prepares the pack's repository, Slack/tracker routing, app-control adapter, model choices, and triage/reproduction automation configuration. |
| [triage-issue-reports](skills/potato-stack/references/pstack/automations/benny/skills/triage-issue-reports/instructions.md) | Reviews a configured Slack report, checks evidence and duplicates, and can deliver one thread verdict plus a justified tracker issue. |
| [reproduce-and-fix-issues](skills/potato-stack/references/pstack/automations/benny/skills/reproduce-and-fix-issues/instructions.md) | Reproduces a trusted triaged symptom in the actual app, verifies existing fixes, and can prepare a bounded draft fix after before/after proof. |

For import versions, host adaptations, and licenses, see the [Potato Stack source notes](skills/potato-stack/references/source.md), [Ponytail source notes](skills/ponytail/references/source.md), and [Cloudflare source notes](skills/cloudflare/references/source.md).
