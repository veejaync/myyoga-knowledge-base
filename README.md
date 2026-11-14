# My Yoga Knowledge Base

A calm, olive-green yoga learning site. Open `index.html` to browse the library; each topic is available as its own page:

- `foundations.html` — Yoga Foundations
- `breath-practice.html` — Breath & Practice
- `flows-reflections.html` — Flows & Reflections
  - `surya-namaskar.html` — a 12-step Surya Namaskar guide with image placeholders
- `asana-benefits.html` — potential benefits across 11 asana categories

The pages share styles from `styles.css` and can be opened locally in a browser.

Asana images are grouped by category in `images/asanas/`. The gallery automatically looks for a JPG matching the pose name in its category folder. Replace a JPG with your own image using the same filename to update that pose; no code change is needed. If an image cannot load, the built-in illustration is shown instead. See [images/asanas/README.md](./images/asanas/README.md) for the pose files and folder names.

Surya Namaskar step photos go in `images/surya-namaskar/`. Name them `step-01.jpg` through `step-12.jpg`, or use the matching `.png` extension. The guide tries JPG first and PNG as a fallback.
