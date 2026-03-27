# HTML/CSS Wireframe

HTML and CSS exercise to recreate a mobile wireframe layout.

> Note: See the [Technical Notes](#technical-notes) section at the end of this document for implementation details and design choices.

## Table of Contents

- [HTML/CSS Wireframe](#htmlcss-wireframe)
  - [Table of Contents](#table-of-contents)
  - [Live Demo](#live-demo)
  - [Run Locally](#run-locally)
  - [Goal](#goal)
  - [Requirements](#requirements)
  - [Project Structure](#project-structure)
  - [Technical Notes](#technical-notes)
  - [Wireframe Example](#wireframe-example)

## Live Demo

[**View Live Demo**](https://emanuelefavero.github.io/htmlcss-wireframe/)

## Run Locally

1. Clone the repository: `git clone https://github.com/emanuelefavero/htmlcss-wireframe.git`
2. Navigate to the project directory: `cd htmlcss-wireframe`
3. Open `index.html` in your web browser to see the wireframe.

> Note: Chrome 112+ is recommended for best CSS nesting support, but any modern browser should work.

## Goal

Reproduce the mobile wireframe shown at the end of this document by building the layout with semantic HTML and CSS. The exercise focuses on the fundamentals of layout composition and visual consistency.

Key areas of attention:

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
├── assets/
│   └── wireframe.webp
├── index.html
├── README.md
└── style.css
```

Main files:

- `index.html` contains the page structure and content.
- `style.css` contains the layout and visual styling rules.
- `assets/wireframe.webp` is the reference wireframe image used for the exercise.

## Technical Notes

- Spacing is applied only between consecutive cards by using a sibling selector.
- Vertical spacing is managed from the parent container instead of assigning top margins directly to each element.
- CSS Nesting is used to keep related selectors grouped together, since it has good support in modern browsers. See [Can I Use](https://caniuse.com/css-nesting) for details.
- `min-height` is used instead of a fixed `height` so the cards can stay visually consistent while still growing when the content is longer.
- A dashed border is kept on `body` to make the simulated viewport clearly visible.

## Wireframe Example

![Wireframe](assets/wireframe.webp)

&nbsp;

---

&nbsp;

[**Go To Top &nbsp; ⬆️**](#htmlcss-wireframe)
