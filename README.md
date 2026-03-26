# HTML/CSS Wireframe

HTML and CSS exercise to recreate a mobile wireframe layout.

> Note: See the [Implementation Notes](#implementation-notes) section at the end of this document for implementation notes and design choices.

## Goal

Reproduce the wireframe shown at the end of this document, with a focus on:

- the box model
- spacing
- consistent layout
- coherent card dimensions

## Requirements

- Set `body { width: 512px; }` to simulate a smartphone screen
- Use the browser inspector to test spacing before updating the code
- Focus on harmonious spacing rather than exact pixel-perfect values
- Keep card heights visually consistent when they contain less text
- Allow cards to grow in height when they contain more text

## Implementation Notes

- Spacing is applied only between consecutive cards by using a sibling selector.
- Vertical spacing is managed from the parent container instead of assigning top margins directly to each element.
- CSS Nesting is used to keep related selectors grouped together, since it is supported in modern browsers.
- `min-height` is used instead of a fixed `height` so the cards can stay visually consistent while still growing when the content is longer.
- A separate `.cards` wrapper was considered, but omitted to keep the structure simpler.
- A dashed border is kept on `body` to make the simulated viewport clearly visible.

## Wireframe

![Wireframe](assets/wireframe.webp)

&nbsp;

---

&nbsp;

[**Go To Top &nbsp; ⬆️**](#htmlcss-wireframe)
