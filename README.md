# Task 4 — Responsive Web Design

## Internship Task

**Web Development Internship — Task 4**

## Objective

This project demonstrates how a desktop-oriented webpage can be converted into a mobile-friendly website using CSS media queries and responsive web design techniques. Because only the official task PDF was provided, the desktop portfolio page was created from scratch and then made responsive.

## Features

- Responsive navigation with a functional mobile menu
- Desktop, tablet and mobile layouts
- Flexible sections using CSS Grid and Flexbox
- Responsive typography using `clamp()` and relative units
- Responsive visual components and images/illustrations contained within their layouts
- Flexible project cards that stack on smaller screens
- Media queries with a primary breakpoint at `768px`
- Responsive spacing using `%`, `rem`, `vw`, `min()`, `max()` and `clamp()` where appropriate
- Mobile-friendly buttons and navigation controls
- Layout designed to prevent horizontal overflow
- Semantic HTML5 structure
- Minimal JavaScript used only for the mobile navigation

## Technologies Used

- HTML5
- CSS3
- CSS Media Queries
- JavaScript

## Responsive Breakpoints

| Breakpoint | Purpose |
|---|---|
| `1024px` | Adjusts desktop spacing and visual sizing for smaller laptop/tablet widths. |
| `768px` | Primary mobile breakpoint. Navigation becomes a functional menu, columns stack, and spacing/layout adapt. |
| `480px` | Optimizes typography, buttons, cards and the hero visual for phones. |
| `340px` | Additional refinement for very small screens such as 320px devices. |

## Testing

The responsive CSS was reviewed against the required viewport sizes and is intended for final verification in Chrome DevTools Device Toolbar at: **1440px, 1200px, 1024px, 768px, 480px, 375px and 320px**.

Checks included:

- Horizontal scrolling / document width
- Navigation behavior
- Text wrapping and overflow
- Card sizing and stacking
- Button usability
- Visual spacing
- Hero visual containment
- Mobile footer layout

## Key Concepts Demonstrated

### Media Queries

CSS `@media` rules change the layout at different viewport widths. The main responsive transformation occurs at `max-width: 768px`.

### Mobile-first vs Desktop-first

This submission starts with a polished desktop-oriented layout and then demonstrates the internship task by adapting it with media queries for smaller screens. This is a desktop-first implementation of the requested conversion exercise.

### Responsive Units

Relative units and functions such as `%`, `rem`, `vw`, `em`, `min()`, `max()` and `clamp()` are used where they provide useful responsive behavior rather than being added artificially.

### Viewport

The page includes the required viewport meta tag so mobile browsers use the device width correctly:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### Flexbox

Flexbox is used for navigation, buttons, metadata, tags and footer alignment. It allows content to wrap or re-align without fixed widths.

### CSS Grid

Grid is used for the main hero, about, skills, projects and contact layouts. Media queries change the number of columns when the available width becomes smaller.

### Responsive Images / Visuals

The stylesheet includes the standard responsive image rule:

```css
img {
  max-width: 100%;
  height: auto;
}
```

The project currently uses CSS-built visual illustrations rather than requiring large external image assets, which keeps the submission lightweight and avoids unnecessary copyrighted assets.

### Adaptive vs Responsive Design

The page continuously adapts its layout, sizing and spacing to the available viewport instead of creating separate fixed pages for individual devices.

## Project Structure

```text
Task-4-Responsive-Website/
│
├── index.html
├── style.css
├── script.js
├── README.md
└── assets/
    └── images/
```

## How to Run

1. Download or clone the repository.
2. Open the project folder in VS Code.
3. Open `index.html` directly in a browser, or use the VS Code Live Server extension if available.
4. Open Chrome DevTools and enable the Device Toolbar.
5. Test the page at different viewport widths.

No build step, package installation or framework is required.

## Personalization

This portfolio is customized for **Rajineni Sreshta**, with web-development-focused skills and representative projects including Annaseva, Book REST API and EduPath.

## What I Learned

This task helped demonstrate how a desktop page can be transformed into a responsive website by identifying layout constraints and adapting them with media queries. It also reinforced the use of flexible Grid/Flexbox layouts, responsive units, viewport configuration, responsive visuals, mobile navigation and overflow prevention.

## GitHub Submission

Create a new GitHub repository for this task and upload the project files, including this README. Do not upload unnecessary cache/build folders.
