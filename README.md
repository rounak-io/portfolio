# Rounak Kumar — Portfolio

**[🔗 Live Demo → rounak-io.github.io/portfolio](https://rounak-io.github.io/portfolio/)**

A minimal, single-file personal portfolio built from scratch with plain HTML, CSS, and vanilla JavaScript. No frameworks, no build step, no dependencies.

I'm a first-year Computer Science student at Sarala Birla University, Ranchi, learning to write software from the ground up: C/C++, data structures, math, and logic.

## Sections

| # | Section | What's inside |
|---|---------|---------------|
| 01 | **Now** | What I'm currently learning: C/C++ fundamentals, data structures, problem solving |
| 02 | **Projects** | Project cards rendered from a JavaScript array (currently placeholders) |
| 03 | **Skills** | An honest inventory: programming, thinking, tools, working style |
| 04 | **Education** | B.Tech in CSE (current), 10+2, 10th |
| 05 | **Contact** | Email, GitHub, LinkedIn, resume download |

## Features

- **Single file**: everything (HTML, CSS, JS, favicon) lives in `portfolio-single.html`
- **Dark theme** with a gold accent and a monospace-driven look
- **Typography**: Space Grotesk for headings, JetBrains Mono for body text (via Google Fonts)
- **Sticky section navigation** that highlights the section you're reading
- **Scroll-reveal and hero animations** using `IntersectionObserver`
- **Accessible**: skip link, visible focus styles, `aria-current` on nav, semantic landmarks
- **Respects `prefers-reduced-motion`**: animations are disabled for users who opt out
- **Responsive** layout with fluid type via `clamp()`
- **Inline SVG favicon**, so no extra image files are needed

## Getting Started

No installation required.

```bash
# Clone the repo
git clone https://github.com/rounak-io/portfolio.git
cd portfolio

# Open in your browser
open portfolio-single.html        # macOS
xdg-open portfolio-single.html    # Linux
start portfolio-single.html       # Windows
```

Or serve it locally:

```bash
python -m http.server 8000
# then visit http://localhost:8000/portfolio-single.html
```

## Customizing

**Add projects**: edit the `PROJECTS` array near the bottom of the file:

```js
var PROJECTS = [
  {
    title: "My Project",
    description: "One-sentence description of what it does.",
    stack: "C / C++",
    learned: "What I figured out while building it.",
    link: "https://github.com/rounak-io/my-project"
    // remove `placeholder: true` for real projects
  }
];
```

**Update links**: replace the `#` placeholders for GitHub and LinkedIn in the hero and Contact sections.

**Resume**: add your PDF at `assets/resume.pdf`, or change the path in the Contact section.

**Colors and spacing**: tweak the CSS variables in the `:root` block at the top of the `<style>` tag (`--bg`, `--text`, `--accent`, etc.).

## Deployment

Since it's a static page, it works on any static host:

- **GitHub Pages**: Settings → Pages → deploy from the `main` branch (rename `portfolio-single.html` to `index.html` so it loads at the root URL)
- **Netlify / Vercel / Cloudflare Pages**: drag and drop the folder or connect the repo

## Tech Stack

- HTML5
- CSS3 (custom properties, flexbox, grid)
- Vanilla JavaScript (ES5-style)

## Contact

- Email: [rounakkumar0042@gmail.com](mailto:rounakkumar0042@gmail.com)
- GitHub: [@rounak-io](https://github.com/rounak-io)
- Live site: [rounak-io.github.io/portfolio](https://rounak-io.github.io/portfolio/)

## License

© 2026 Rounak Kumar. All rights reserved. Feel free to take inspiration from the design, but please don't copy the content as your own.
