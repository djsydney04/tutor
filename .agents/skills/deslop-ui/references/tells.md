# UI patterns worth questioning

Read this through [deslop-ui](../SKILL.md). These are prompts for judgment, not
evidence of authorship. An intentional brand treatment or useful convention can
pass. A finding needs a location, an actual cost, and a better alternative.

## Page structure and product identity

| Candidate pattern | Why to inspect it | Purposeful alternative or legitimate use |
| --- | --- | --- |
| A page built from the same hero, equal feature tiles, numbers, pricing, and FAQ regardless of the product | The assembly can hide the real offer behind interchangeable sections. | Organize around the buyer's questions and actual product evidence. Keep sections that answer a real question. |
| Every section uses the same alignment, label, heading, and grid | Equal emphasis makes the page's priorities hard to read. | Change scale and composition with importance. Repeat structure when items genuinely need comparison. |
| Every item is boxed, including boxes inside boxes | Container boundaries can replace meaningful grouping and add scanning work. | Group with alignment, space, and type. Keep containers for distinct objects, interactions, or ownership. |
| A stock component kit supplies the entire identity | Default styling can leave brand and hierarchy decisions unresolved. | Keep accessible primitives and choose coherent tokens, density, emphasis, and product-specific content. |
| Another company's visual language transplanted wholesale | Recognition can belong to the reference instead of the product. | Borrow a useful principle and express it through the target's own brand. Match an ecosystem when that is the real requirement. |
| A mock terminal, dashboard, or chart has no explanatory role | Decorative complexity can imply functionality or evidence that does not exist. | Show real output, a clearly labeled illustration, or a simpler explanation. Demos should explain a true capability. |

## Typography, color, and surfaces

| Candidate pattern | Why to inspect it | Purposeful alternative or legitimate use |
| --- | --- | --- |
| Luminous text, background haze, glass, or grids applied throughout | Competing effects can weaken contrast and distract from the offer. | Establish a quiet hierarchy and use effects where they explain layering or carry an intentional brand idea. |
| Very round shapes, floating pills, or accent borders on everything | Repeated emphasis can make unrelated things look equally important. | Define shape and emphasis roles. Preserve selected-state indicators and meaningful labels. |
| Tiny spaced capitals for every secondary label | Styling can reduce readability and add visual noise without clarifying structure. | Use legible labels and deliberate type hierarchy. Keep established brand typography when it works. |
| Every work surface has promotional-scale whitespace | Low density can push related information apart and slow repeated tasks. | Tune density to reading, comparison, and editing; give a marketing statement room when it needs it. |
| A fashionable font or palette substitutes for a direction | A cosmetic swap leaves the underlying hierarchy unresolved. | Choose typography and color roles based on content, platform, and brand; check the actual result. |

## Signals, motion, and copy

| Candidate pattern | Why to inspect it | Purposeful alternative or legitimate use |
| --- | --- | --- |
| Pulsing dots, decorative gauges, or fake keyboard hints | They can imply state or functionality the interface does not provide. | Tie signals to real data and working actions. Use stable labels; animate real changes only when useful. |
| Every surface moves on hover or appears through a scroll effect | Motion can delay access, hide content, and compete for attention. | Animate meaningful transitions, preserve usable static content, and honor reduced motion. |
| Generic symbols repeated above every feature | The imagery can consume space without helping users distinguish capabilities. | Use precise labels, relevant product imagery, or icons that improve recognition. |
| Slogans that could describe any product | Abstract promises make the actual capability and next action unclear. | Name the operation, audience, constraint, or outcome in concrete language. Keep the product's voice. |
| Invented people, customer logos, usage totals, or performance claims | Fabricated proof misleads users regardless of visual quality. | Use substantiated evidence or omit the claim. Mark illustrative data as sample content in prototypes. |
| Empty badges, release labels, countdowns, or atmospheric metadata | Decorative detail can manufacture urgency or imply context that is irrelevant. | Keep real release/state information where it helps a decision; remove filler. |

## Apply the checklist with context

- A service-health view can need status badges and time labels. Inspect whether
  they encode real states before suggesting removal.
- A purple brand can use purple, and a specification table can use separators.
  Judge hierarchy, legibility, and consistency rather than a prohibited color
  or CSS property.
- A marketing screenshot can illustrate an app, but it does not establish that
  the pictured workflow works. Separate explanation from interaction evidence.
- An accessible navigation component can be familiar and still be the right
  choice. Keep its behavior when changing visual styling.

See [source notes](../../design-taste/references/sources.md). This checklist is
an original synthesis, not a copy of an upstream ban list.
