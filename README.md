# SASS Landing Page

A responsive landing page refactored from plain CSS to **SASS (SCSS)** using variables, nesting, mixins and partials. The compiled page looks and behaves the same as the original, but the styles are easier to read, reuse and maintain.

**Author:** Pratiksha Bhende
**GitHub:** [pratiksha0604](https://github.com/pratiksha0604)

## Features

- Responsive layout (desktop, tablet and mobile)
- Sticky navbar with smooth scrolling to each section
- Hero section with a call-to-action button
- Feature cards that stack on smaller screens
- Contact footer

## What was refactored with SASS

| SASS feature | How it is used |
|---|---|
| Variables | Colors, spacing, fonts and breakpoints are stored in `_variables.scss` |
| Nesting | Navbar, hero, features and footer rules are nested |
| Mixins | `flex-center`, `flex-between`, `button()` and `respond()` remove repeated code |
| Partials | Styles are split into `_variables.scss`, `_mixins.scss` and `style.scss` |

## Tech Stack

- HTML5
- SASS / SCSS
- Node.js and npm
- Git and GitHub

## Project Structure

```
sass-landing-page/
├── css/
│   └── style.css
├── scss/
│   ├── _variables.scss
│   ├── _mixins.scss
│   └── style.scss
├── index.html
├── package.json
├── .gitignore
└── README.md
```

## Getting Started

```bash
git clone https://github.com/pratiksha0604/sass-landing-page.git
cd sass-landing-page
npm install
```

### Compile SASS

```bash
npm run sass     # compile once
npm run watch    # recompile on every save
```

Then open `index.html` in your browser.

## Responsive Breakpoints

| Breakpoint | Width | Behavior |
|---|---|---|
| Tablet | 768px and below | Navbar and cards stack |
| Mobile | 480px and below | Smaller hero heading |

## License

ISC