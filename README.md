# axellee1994.github.io

A small, static personal portfolio / project site built with plain HTML, Tailwind utilities (via CDN), and a handful of local CSS files.

Quick facts
- Static site — no build step required.
- Edit pages in `frontend/pages/` and global styles in `frontend/assets/main.css`.

Repository layout (important files)
- `index.html` — landing page (hero, about, projects, contact, footer).
- `frontend/assets/main.css` — centralized site styles and variables.
- `frontend/assets/project_page.css` — project-page specific overrides (imports `main.css`).
- `frontend/pages/` — individual project pages (`project1.html`, `project2.html`, `project3.html`).
- `frontend/assets/JPEG/` — place hero images here (e.g. `Hero-2400.jpg`) for responsive hero backgrounds.

Preview locally
1. From the repo root run a simple static server and open http://localhost:8000

```bash
# Python 3
python3 -m http.server 8000
```

Developer notes
- Navigation and footer are shared across pages; update `index.html` to change site-wide headings/links and copy to project pages if needed.
- Tailwind: the site currently uses a CDN (older v2/v3 variants may exist in files). If you want newer Tailwind utilities, consider switching to the Play CDN or adding a local build step.
- Animations: animate.css and a small IntersectionObserver-based scroll-reveal script are used — these are included in the pages.
- Accessibility: there is a skip link and prefers-reduced-motion support in CSS. Keep animation durations respectful.

Contributing
- Open a PR with small, focused changes. For visual tweaks, include screenshots and the browser/OS used.

Contact
- For quick edits, modify the files above and preview locally using the static server command.

License
- This repo has no license file. Add a LICENSE if you want to make the project open-source.