# My Yoga Knowledge Base

A calm, olive-green yoga learning site. Open `index.html` to browse the library; each topic is available as its own page:

- `foundations.html` — Yoga Foundations
- `breath-practice.html` — Breath & Practice
- `flows-reflections.html` — Flows & Reflections
- `asana-benefits.html` — potential benefits across 11 asana categories

The pages share styles from `styles.css` and can be opened locally in a browser.

Asana photos are grouped by category in `images/asanas/`. To replace a pose illustration, put its JPG in the matching category folder, then add its pose name and path to the `posePhotos` object in `asana-benefits.html`, for example:

```js
const posePhotos = {
  "Tree Pose": "images/asanas/balancing/tree-pose.jpg"
};
```

The pose name must match the gallery entry. Unmapped poses keep their vector illustrations; if a mapped image cannot load, the page reports it and keeps the illustration visible. See [images/asanas/README.md](./images/asanas/README.md) for category folders and pose filenames.
