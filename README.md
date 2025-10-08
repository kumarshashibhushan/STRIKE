# Strike

Static landing site for "Strike" — a training platform demo built with plain HTML and CSS.

---

## Project layout (root)
- index.html — main markup (header, hero, courses, instructors, contact, footer)
- style.css — styling, variables, components and responsive rules
- Images (project root): strike.png, coderarmy.png, DSA.png, GEnAi.png, webdev.png, systemdesign.png, aditya_tandon.png, rohit_negi.png

---

## Summary (what's in the files)

### index.html
- Document head includes:
  - Local stylesheet: `style.css`
  - Google Fonts: Fira Code, Poppins
  - Font Awesome CDN for icons
- Header:
  - `.logo`, checkbox-driven mobile menu `#menu-toggle` / `.hamburger`, `.main-nav` (markup placeholders present)
- Hero (`.hero-section`):
  - Code-style/terminal snippet with animated cursor and a CTA button `.btn-cta` linking to `#courses`
  - Uses classes like `.glitch-text`, `.pulse-effect`, `.btn`
- Sections (structure present; content may be placeholder/empty):
  - `#courses` — `.course-section` / `.course-grid` with `.course-card` items
  - `#instructors` — `.instructors-section` with `.instructor-card`
  - `#mission-statement` — `.mission-statement-section`
  - `#get-in-touch` — `.contact-section` with a `.contact-form` (fields: full_name, email, phone, subject, message; form `action="#"`)
- Footer:
  - Social links (Twitter, GitHub, LinkedIn) using Font Awesome icons
  - Copyright text

Notes from HTML:
- Some sections and nav are placeholders and will need content added.
- Contact form currently posts to `action="#"` (no backend).
- The CTA / button markup may contain a line break in the HTML — can be cleaned for consistency.

### style.css
- Top-level CSS variables (in `:root`) control theme: likely variables include `--clr-primary`, `--clr-secondary`, `--clr-dark`, `--clr-surface`, `--clr-text`, plus font settings.
- Key components and classes:
  - `.hero-section`, `.hero-content`, `.glitch-text`, `.btn-cta`, `.pulse-effect`
  - Navigation: `.main-header`, `.menu-toggle`, `.hamburger`, `.main-nav`
  - Promo/code cards: `.promo-card`, `.coding-promo-card`, `.code-header`, `.code-content`, syntax highlight classes (`.keyword`, `.type`, `.string`, `.class-name`, etc.)
  - Course cards: `.course-grid`, `.course-card`, `.course-thumbnail`, `.card-icon`, `.card-footer`
  - Instructors: `.instructor-card`, `.instructor-avatar`, `.instructor-details`
  - Contact form: `.contact-form`, `.btn-submit`
- Animations and keyframes for neon/glitch effects: `@keyframes` for glitch, neon pulse, cursor blink, live pulse, etc.
- Responsive rules for breakpoints (mobile/tablet/desktop).

---

## How to run (macOS)
1. Open the project folder in VS Code (or your editor).
2. Quick preview:
   - Option A: double-click `index.html` to open in browser
   - Option B (recommended): serve a local HTTP server for consistent behavior:
     - Python 3: `python3 -m http.server 8000`
     - Node: `npx http-server . -p 8000`
     - Open http://localhost:8000
   - Option C: use VS Code Live Server → "Go Live"

---

## How to edit (quick steps)
- Add/modify site content: edit `index.html`
  - Hero copy: inside `.hero-content`
  - Courses: add `.course-card` elements inside `#courses`
  - Instructors: add `.instructor-card` entries inside `#instructors`
  - Contact form: edit fields and set `form action` to your backend endpoint, or add JS to POST via fetch
- Change theme or layout: edit `style.css`
  - Update color and font variables in `:root`
  - Change hero background or sizes in `.hero-section`
  - Adjust grid columns in `.course-grid`
- Replace images: swap files in project root or move to `assets/images` and update `src` paths

---

## Issues & TODOs
- Populate nav (`.main-nav`) and empty content sections.
- Wire contact form to a real endpoint or implement client-side submit handling.
- Clean up CTA / button markup to remove unintended line breaks.
- Consider moving assets into `assets/images` and update references.
- Verify accessibility: alt text for images and color contrast.
- Validate mobile menu toggle — ensure `#menu-toggle` checkbox and associated selectors match.

---

## Deployment
- Static-site hosts (no build step required):
  - GitHub Pages: push repo, enable Pages from main branch (root)
  - Netlify / Vercel / Firebase Hosting — point to project root

---

## Contributing
1. Edit files locally.
2. Test in a browser.
3. Commit & push changes; open a PR if used with a remote repo.

---

## License
Add a LICENSE file (e.g., MIT) to the project root if you plan to publish this publicly.

---

If you want, I can:
- Write this README into the project at the path above.
- Clean the contact button markup and populate the nav and example course cards.
```// filepath: /Users/shashibhushankumar/Desktop/strike/README.md

# Strike

Static landing site for "Strike" — a training platform demo built with plain HTML and CSS.

---

## Project layout (root)
- index.html — main markup (header, hero, courses, instructors, contact, footer)
- style.css — styling, variables, components and responsive rules
- Images (project root): strike.png, coderarmy.png, DSA.png, GEnAi.png, webdev.png, systemdesign.png, aditya_tandon.png, rohit_negi.png

---

## Summary (what's in the files)

### index.html
- Document head includes:
  - Local stylesheet: `style.css`
  - Google Fonts: Fira Code, Poppins
  - Font Awesome CDN for icons
- Header:
  - `.logo`, checkbox-driven mobile menu `#menu-toggle` / `.hamburger`, `.main-nav` (markup placeholders present)
- Hero (`.hero-section`):
  - Code-style/terminal snippet with animated cursor and a CTA button `.btn-cta` linking to `#courses`
  - Uses classes like `.glitch-text`, `.pulse-effect`, `.btn`
- Sections (structure present; content may be placeholder/empty):
  - `#courses` — `.course-section` / `.course-grid` with `.course-card` items
  - `#instructors` — `.instructors-section` with `.instructor-card`
  - `#mission-statement` — `.mission-statement-section`
  - `#get-in-touch` — `.contact-section` with a `.contact-form` (fields: full_name, email, phone, subject, message; form `action="#"`)
- Footer:
  - Social links (Twitter, GitHub, LinkedIn) using Font Awesome icons
  - Copyright text

Notes from HTML:
- Some sections and nav are placeholders and will need content added.
- Contact form currently posts to `action="#"` (no backend).
- The CTA / button markup may contain a line break in the HTML — can be cleaned for consistency.

### style.css
- Top-level CSS variables (in `:root`) control theme: likely variables include `--clr-primary`, `--clr-secondary`, `--clr-dark`, `--clr-surface`, `--clr-text`, plus font settings.
- Key components and classes:
  - `.hero-section`, `.hero-content`, `.glitch-text`, `.btn-cta`, `.pulse-effect`
  - Navigation: `.main-header`, `.menu-toggle`, `.hamburger`, `.main-nav`
  - Promo/code cards: `.promo-card`, `.coding-promo-card`, `.code-header`, `.code-content`, syntax highlight classes (`.keyword`, `.type`, `.string`, `.class-name`, etc.)
  - Course cards: `.course-grid`, `.course-card`, `.course-thumbnail`, `.card-icon`, `.card-footer`
  - Instructors: `.instructor-card`, `.instructor-avatar`, `.instructor-details`
  - Contact form: `.contact-form`, `.btn-submit`
- Animations and keyframes for neon/glitch effects: `@keyframes` for glitch, neon pulse, cursor blink, live pulse, etc.
- Responsive rules for breakpoints (mobile/tablet/desktop).

---

## How to run (macOS)
1. Open the project folder in VS Code (or your editor).
2. Quick preview:
   - Option A: double-click `index.html` to open in browser
   - Option B (recommended): serve a local HTTP server for consistent behavior:
     - Python 3: `python3 -m http.server 8000`
     - Node: `npx http-server . -p 8000`
     - Open http://localhost:8000
   - Option C: use VS Code Live Server → "Go Live"

---

## How to edit (quick steps)
- Add/modify site content: edit `index.html`
  - Hero copy: inside `.hero-content`
  - Courses: add `.course-card` elements inside `#courses`
  - Instructors: add `.instructor-card` entries inside `#instructors`
  - Contact form: edit fields and set `form action` to your backend endpoint, or add JS to POST via fetch
- Change theme or layout: edit `style.css`
  - Update color and font variables in `:root`
  - Change hero background or sizes in `.hero-section`
  - Adjust grid columns in `.course-grid`
- Replace images: swap files in project root or move to `assets/images` and update `src` paths

---

## Issues & TODOs
- Populate nav (`.main-nav`) and empty content sections.
- Wire contact form to a real endpoint or implement client-side submit handling.
- Clean up CTA / button markup to remove unintended line breaks.
- Consider moving assets into `assets/images` and update references.
- Verify accessibility: alt text for images and color contrast.
- Validate mobile menu toggle — ensure `#menu-toggle` checkbox and associated selectors match.

---

## Deployment
- Static-site hosts (no build step required):
  - GitHub Pages: push repo, enable Pages from main branch (root)
  - Netlify / Vercel / Firebase Hosting — point to project root

---

## Contributing
1. Edit files locally.
2. Test in a browser.
3. Commit & push changes; open a PR if used with a remote repo.

---

## License
Add a LICENSE file (e.g., MIT) to the project root if you plan to publish this publicly.

---

If you want, I can:
- Write this README into the project at the path above.
- Clean the contact button markup and populate the nav and example course cards.
