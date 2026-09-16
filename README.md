# Ahmad Alhwari — Personal Portfolio

A fully responsive personal portfolio website built with semantic HTML and CSS.
It serves as a live resume showcasing my background, skills, and selected projects.

**Live site:** https://ahmad-alhwari0.github.io/Portfolio-project/

---

## Overview

This project was built as a capstone for the HTML/CSS module. The goal was to
create a professional, accessible, and fully responsive portfolio, writing all
layout and styling by hand rather than relying on a CSS framework or page builder.

Bootstrap is included for one purpose only — the collapsible mobile navigation,
which requires JavaScript to toggle. Everything else is custom CSS.

The design was planned first as a wireframe, then as a high-fidelity mockup in
Figma, before any code was written.

---

## Features

- **Semantic HTML5 structure** — `header`, `main`, `section`, `article`, `footer`, `dl`
- **CSS Grid and Flexbox layouts** — Grid for two-dimensional sections, Flexbox for single-axis groups
- **Fully responsive** — two breakpoints (1024px / 768px) covering desktop, tablet, and mobile
- **BEM naming convention** — scalable, readable class names throughout
- **CSS custom properties** — colors and layout values defined once in `:root`
- **Transitions and hover states** on all interactive elements
- **Keyframe animation** on the hero section
- **Accessible** — `aria-label` on icon links, labeled form fields, `prefers-reduced-motion` support
- **Working contact form** via Formspree
- **Collapsible mobile navigation**
- **Smooth scrolling** between sections

---

## Sections

| Section | Description |
|---|---|
| Hero | Introduction, role, and primary call to action |
| About | Background and professional summary |
| Projects | Selected work with details and repository links |
| Capabilities | Technical skills grouped by category |
| Contact | Contact details and a working message form |
| Footer | Copyright |

---

## Tech Stack

- HTML5
- CSS3 (Grid, Flexbox, custom properties, media queries)
- Bootstrap 5 — collapsible mobile navigation only
- Font Awesome — icons
- Google Fonts (Inter) — typography
- Formspree — contact form handling

---

## Project Structure

```
Portfolio-project/
├── index.html
├── README.md
├── .gitignore
├── css/
│   └── style.css
├── image/
│   ├── ahmdalhwari.jpeg
│   ├── project1.png
│   ├── project2.png
│   └── comingsoon.png
├── files/
│   └── Ahmad_Alhwari.pdf
└── documentation/
    ├── wireframe-desktop-mobile.png
    └── mockup-desktop-mobile.png
```

---

## How to Run

**Option 1 — Open directly**

```bash
git clone https://github.com/Ahmad-alhwari0/Portfolio-project.git
cd Portfolio-project
```

Then open `index.html` in any browser.

**Option 2 — Live Server (recommended)**

Open the folder in VS Code, install the *Live Server* extension, right-click
`index.html` and choose **Open with Live Server**.

No build step or dependencies are required.

---

## Design Decisions

**Semantic markup over generic containers.** Each project card is an `<article>`
because it is self-contained content that would still make sense in isolation.
Project metadata uses a description list (`<dl>` / `<dt>` / `<dd>`) rather than a
table, since the data is key–value pairs rather than tabular data.

**`position: sticky` for the header.** Unlike `fixed`, sticky keeps the element in
the document flow, so no compensating padding is needed on the body.

**Grid vs Flexbox.** Grid is used where the layout is two-dimensional or the
column count is fixed (hero, project cards, skill groups). Flexbox is used where
items sit on a single axis and the count varies (navigation, skill tags, action
groups).

**Desktop-first responsive approach.** The base styles target desktop, with
`max-width` media queries collapsing multi-column layouts into a single column
below 768px.

**Shared utility classes.** Repeated patterns — buttons, social icon groups,
section titles — were extracted into `.btn`, `.social`, and `.section-title`
instead of being duplicated per section.

---

## Author

**Ahmad Alhwari** — Full-Stack Developer, Jordan

- GitHub: [@Ahmad-alhwari0](https://github.com/Ahmad-alhwari0)
- LinkedIn: [ahmad-alhwari](https://linkedin.com/in/ahmad-alhwari-17a3a0371)
- Email: ahmadalhwari0@gmail.com