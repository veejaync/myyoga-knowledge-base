# My Yoga Knowledge Base

A calm, olive-green yoga learning site. Open `index.html` to browse the library; each topic is available as its own page:

- `foundations.html` — Yoga Foundations
- `breath-practice.html` — Breath & Practice
- `flows-reflections.html` — Flows & Reflections
  - `surya-namaskar.html` — a 12-step Surya Namaskar guide with image placeholders
- `asana-benefits.html` — potential benefits across 11 asana categories

The pages share styles from `styles.css`. To browse the site locally, start a web server from the project folder:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open `http://localhost:8000`. The Asana page fetches its content from JSON, so it must be opened through a web server rather than directly as a `file://` URL.

## Editing Asana content

The categories, benefit notes, and pose details for `asana-benefits.html` are stored in [`data/asana-benefits.json`](./data/asana-benefits.json). Edit the `categories` array to change the page content or order. Each category has an `id`, display labels, benefit notes, and a `poses` array. The category `id` also names its folder under `images/asanas/`; pose photos use a lowercase hyphenated version of the pose name, with `.jpg` preferred and `.png` as a fallback. The `head` and `figure` pose fields define the built-in illustration shown when neither photo is available. Keep the file valid JSON when editing it.

Asana images are grouped by category in `images/asanas/`. The gallery tries a JPG matching the pose name first, then a PNG with the same filename in its category folder. Use either format; if both are present, JPG is used. If neither image loads, the built-in illustration is shown. See [images/asanas/README.md](./images/asanas/README.md) for pose filenames and folders.

Surya Namaskar step photos go in `images/surya-namaskar/`. Name them `step-01.jpg` through `step-12.jpg`, or use the matching `.png` extension. The guide tries JPG first and PNG as a fallback.
