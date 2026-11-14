---
name: design-taste
description: Choose and carry through a deliberate visual direction for landing pages, websites, and product interfaces. Use for art direction, visual polish, taste, or applying the user's design references; preserve existing brand systems and the requested critique, plan, or implementation mode.
---

# Design taste

Make visual choices that belong to this product and help its users. Taste means
coherent judgment about what to emphasize, what to simplify, and what fits.
Use this with [Designer](../persona-designer/SKILL.md) when the work also needs
journeys or interaction design. Read the relevant section once; routine fixes
inside an established system need no new art direction.

## Establish the direction

1. Read the target project's instructions, current interface, components, and
   brand guidance. Identify the audience, task, surface, platform, real content,
   and constraints. Preserve the current system unless a redesign is requested.
2. Open the [reference index](references/design-index.md). Choose one primary
   reference for structure and, if useful, one supporting reference for a
   specific detail. Match the surface and user task before the visual mood.
   The index distinguishes user preferences from interpretations.
3. Inspect the chosen page or supplied screenshot before making detailed visual
   claims. Note the URL, section, viewport, date, and what was actually visible.
   An inaccessible page can remain a bookmark; it is not observed evidence.
4. State a short direction in the task or existing design document: who it is
   for, the visual character, and the product-specific reason it fits. Identify
   the hierarchy, typography, palette, density, imagery, and motion that matter
   here. Use concrete decisions rather than adjectives such as "premium."
5. Carry over principles such as alignment, pacing, or product demonstration.
   Use the target's content and identity. Do not copy another company's mark,
   copy, assets, or entire visual language. Compare alternatives only when a
   meaningful design choice remains unresolved.

For example: "A deployment console for engineers scanning failures: compact
rows, aligned numbers, quiet surfaces, and color reserved for state. Borrow
Railway's idea of making relationships legible, using our existing components."
This is a direction to verify, not a claim about Railway's current console.

## Make the choices concrete

| Decision | What to resolve |
| --- | --- |
| Hierarchy | What gets attention first, what supports it, and what can recede? Make the main action and essential information easy to locate. |
| Typography | Choose roles, sizes, weights, line length, and wrapping for real content. Use existing or licensed fonts; a new font is not a substitute for hierarchy. |
| Layout and density | Align related elements and use repeatable spacing. Let reading, comparison, and frequent work determine density. |
| Color and shape | Define surface, text, accent, focus, and semantic state roles with a consistent radius and border system. Distinguish states beyond color alone. |
| Imagery and evidence | Use actual product output or relevant, authorized imagery. State what is illustrative; keep claims and testimonials verifiable. |
| Interaction and motion | Make affordances and feedback clear. Use motion to explain a change, respect reduced motion, and keep the task usable without animation. |

Keep the established framework, accessible primitives, and working interactions.
Use the project's tokens and components before adding new ones. Choosing a
direction does not require installing a style package, animation library, image
generator, or font service.

## Adapt to the surface

- **Landing pages:** organize the argument around the offer, product evidence,
  useful explanation, trust, and a next step. Give each section a reason to exist
  and vary emphasis with importance. Avoid inventing content to fill a template.
- **Product interfaces:** organize around the work. Support scanning, selection,
  editing, comparison, and recovery with clear labels and stable navigation.
  Use representative content and cover long values, empty/loading/error states,
  and permissions where relevant. Keep charts tied to meaningful data.
- **Native interfaces:** preserve platform conventions and the app's design
  system. Translate a reference's principle into native components rather than
  imposing a marketing page's layout on a task screen.

## Evaluate the result

Inspect the actual artifact at the relevant small and large viewports. For a
working UI, exercise navigation, primary actions, keyboard focus, and affected
states; inspect screenshots for hierarchy, alignment, type wrapping, contrast,
image crops, and unnecessary decoration. Include reduced motion where affected.
Use [deslop-ui](../deslop-ui/SKILL.md) for a focused check of generic patterns.
Fix the highest-impact mismatches before adding detail.

Report the chosen direction, the reference principle used, what changed or is
proposed, and what was verified. A text or source review cannot establish rendered
quality, accessibility compliance, or usability. If browser access is unavailable,
continue the useful scoped work and state that rendered verification remains.

Preserve the requested mode: critique and planning do not authorize edits;
implementation follows existing authorization. Reference browsing does not
authorize importing assets, installing plugins, publishing, or changing accounts.
Resolve links from this file's canonical location when accessed through a symlink.
See [source notes](references/sources.md) for the supplied inspirations and limits.
