# SASS Landing Page

A responsive landing page refactored from plain CSS to **SASS (SCSS)**, using variables, nesting, mixins and partials. The compiled page looks and behaves the same as the original, but the styles are now easier to read, reuse and maintain.

**Author:** Pratiksha Bhende
**GitHub:** [pratiksha0604](https://github.com/pratiksha0604)

---

## Features

- Responsive layout (desktop, tablet and mobile)
- Sticky navbar with smooth scrolling to each section
- Hero section with a call-to-action button
- Feature cards that stack on smaller screens
- Contact footer

## What was refactored with SASS

| SASS feature | How it is used |
|---|---|
| **Variables** | Colors, spacing, fonts, border radius and breakpoints are stored in `_variables.scss` |
| **Nesting** | Navbar, hero, features and footer rules are nested instead of repeating selectors |
| **Mixins** | `flex-center`, `flex-between`, `button()` and `respond()` remove repeated code |
| **Partials** | Styles are split into `_variables.scss`, `_mixins.scss` and `style.scss` |
| **`@use`** | Partials are imported into the main file with the modern module system |

## Tech Stack

- HTML5
- SASS / SCSS
- Node.js and npm (to install and run Sass)
- Git and GitHub

## Project Structure

```
sass-landing-page/
├── css/
│   └── style.css          # compiled CSS (generated)
├── scss/
│   ├── _variables.scss    # colors, spacing, breakpoints
│   ├── _mixins.scss       # reusable mixins
│   └── style.scss         # main stylesheet (nesting + imports)
├── index.html
├── package.json
├── .gitignore
└── README.md
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (includes npm)
- [Git](https://git-scm.com/)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/pratiksha0604/sass-landing-page.git

# 2. Go into the project folder
cd sass-landing-page

# 3. Install dependencies
npm install
```

### Compile SASS

```bash
# Compile once
npm run sass

# Watch for changes and recompile automatically
npm run watch
```

### View the page

Open `index.html` in your browser (double-click it, or use the VS Code **Live Server** extension).

## Available Scripts

| Command | Description |
|---|---|
| `npm run sass` | Compiles `scss/style.scss` into `css/style.css` |
| `npm run watch` | Watches the SCSS files and recompiles on every save |

## Responsive Breakpoints

| Breakpoint | Width | Behavior |
|---|---|---|
| Desktop | above 768px | Navbar in one row, cards side by side |
| Tablet | 768px and below | Navbar stacks, cards stack vertically |
| Mobile | 480px and below | Smaller hero heading |

## Git Workflow Used

```bash
git init
git add .
git commit -m "Refactor responsive landing page using SASS"
git branch -M main
git remote add origin https://github.com/pratiksha0604/sass-landing-page.git
git push -u origin main
```

## License

This project is licensed under the ISC License.