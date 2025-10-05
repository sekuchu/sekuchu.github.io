# sekuchu.github.io

This repository powers my personal portfolio hosted with GitHub Pages. It contains the HTML, CSS, JavaScript, and assets used to showcase my work, experience, and contact information.

## Local development

Clone the repository and serve it with any static file server. One simple option is Python's built-in HTTP server:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## Structure

- `index.html` – the main single-page portfolio experience.
- `assets/css/` – styles for the site.
- `assets/js/` – JavaScript for interactive components such as navigation and filtering.
- `assets/images/` – profile pictures, project thumbnails, and icons.
- `backup/` – snapshots of the original files before the current redesign.

## Content quickstart

Most of the copy lives in `index.html`. To update it quickly:

1. **About & wins** – edit the "About me" paragraphs and the `.wins` list to spotlight new outcomes or metrics.
2. **Resume timeline** – adjust the `<ol class="timeline-list">` entries under the "Education" and "Experience" sections.
3. **Projects** – each `.project-item` contains a title, category, link, image, and a short summary line. Swap in new work by updating the anchor tag and thumbnail path.
4. **Contact actions** – tweak the call-to-action buttons or update the availability statements inside the `.contact-actions` section.

For larger edits, consider duplicating `index.html` to a temporary file so you can preview changes side-by-side before publishing.

## Visual polish

- `assets/css/style.css` contains reusable gradients, spacing tokens, and breakpoints. The new `.wins-` and `.skills-` components use the same gradient border treatment as service cards so the site stays cohesive.
- `assets/js/script.js` powers navigation, project filtering, and (optionally) testimonials. The logic is now defensive, so unused components can be removed without triggering errors.

## License

Content is © Branko Sekulović. Code is released under the MIT License – see [`LICENSE`](LICENSE).
