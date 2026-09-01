# faiz2602.github.io

Source for my personal portfolio site, published via GitHub Pages at **[faiz2602.github.io](https://faiz2602.github.io)**.

It's a single self-contained `index.html` — no build step, no framework, no dependencies beyond a couple of CDN-hosted fonts/icons — covering my background, publications, patent and design registration, awards, and current projects as a Computer Science & AI undergraduate at VIT Bhopal University.

## Structure

The page is one long scroll broken into sections, each independently linkable:

| Section | Anchor | Content |
|---|---|---|
| About | `#about` | Background, research focus, and a skills strip |
| Publications | `#publications` | Journal/conference papers, most recent first |
| Patents & Design Registration | `#ip` | The published utility patent and granted design registration for the structural crack-monitoring device, with links to the official certificates |
| Awards & Recognition | `#awards` | A timeline of awards and milestones |
| Current Work | `#projects` | Active/shipped projects, each as a "spotlight" card with milestones, tech stack, and links |
| Profiles & Contact | `#contact` | Email, LinkedIn, ORCID, Google Scholar, Semantic Scholar |

Everything lives in `index.html`: HTML, CSS (in a single `<style>` block using CSS custom properties for the color palette), and the small amount of JavaScript that drives the mobile nav, on-scroll reveal animations, and the cursor glow effect.

## Assets

- `Portrait.JPG` — profile photo used in the hero section
- `patent_certificate.jpg`, `patent_recognition.pdf` — official Indian Patent Office application record
- `design_certificate.jpg`, `design_cert-1.jpg`, `design_recognition.pdf` — official Certificate of Registration of Design
- `front.jpg`, `back.jpg`, `left.jpg`, `right.jpg`, `top.jpg`, `bottom.jpg`, `section.jpg`, `perspective.jpg` — granted design-registration views of the physical crack-monitoring device
- `prototype.jpg` — the assembled physical prototype

## Running locally

No build step is required — just open the file directly:

```
git clone https://github.com/Faiz2602/Faiz2602.github.io.git
cd Faiz2602.github.io
open index.html   # or: python3 -m http.server, then visit localhost:8000
```

## Deployment

The site deploys automatically via **GitHub Pages** from the `main` branch — any push here goes live at faiz2602.github.io within a minute or two.

## Updating content

Since everything is in one file, adding a new project or publication means adding another `.card` or `.spotlight` block inside the relevant `<section>`, following the existing markup pattern for that section (see the CSS class names — `.card`, `.spotlight`, `.milestones`, `.chip`, `.tag` — defined at the top of `index.html`).
