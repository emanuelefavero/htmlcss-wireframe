# HTML/CSS Wireframe

HTML and CSS exercise to recreate a mobile wireframe layout.

> Note: See the [Implementation Notes](#implementation-notes) section at the end of this document for implementation notes and design choices.

## Table of Contents

- [HTML/CSS Wireframe](#htmlcss-wireframe)
  - [Table of Contents](#table-of-contents)
  - [Live Demo](#live-demo)
  - [How to run the project](#how-to-run-the-project)
  - [Goal](#goal)
  - [Requirements](#requirements)
  - [Project Structure](#project-structure)
  - [Implementation Notes](#implementation-notes)
  - [Wireframe example](#wireframe-example)

## Live Demo

[**View Live Demo**](https://emanuelefavero.github.io/htmlcss-wireframe/)

## How to run the project

1. Clone the repository: `git clone https://github.com/emanuelefavero/htmlcss-wireframe.git`
2. Navigate to the project directory: `cd htmlcss-wireframe`
3. Open `index.html` in your web browser to see the wireframe.

> Note: Chrome 112+ is recommended for best CSS support, but any modern browser should work.

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

## Project Structure

```txt
htmlcss-wireframe/
├── index.html
└── styles.css
```

## Implementation Notes

- Spacing is applied only between consecutive cards by using a sibling selector.
- Vertical spacing is managed from the parent container instead of assigning top margins directly to each element.
- CSS Nesting is used to keep related selectors grouped together, since it is supported in modern browsers.
- `min-height` is used instead of a fixed `height` so the cards can stay visually consistent while still growing when the content is longer.
- A separate `.cards` wrapper was considered, but omitted to keep the structure simpler.
- A dashed border is kept on `body` to make the simulated viewport clearly visible.

## Wireframe example

![Wireframe](assets/wireframe.webp)

&nbsp;

---

&nbsp;

[**Go To Top &nbsp; ⬆️**](#htmlcss-wireframe)
