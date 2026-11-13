# Asana photo folders

Put each JPG in the folder for its category. Use the pose filename shown below:

| Category folder | Pose image filenames |
|---|---|
| `balancing/` | `tree-pose.jpg`, `dancer-pose.jpg`, `eagle-pose.jpg` |
| `inversions/` | `downward-facing-dog.jpg`, `legs-up-the-wall.jpg`, `shoulderstand.jpg` |
| `core/` | `plank-pose.jpg`, `boat-pose.jpg`, `side-plank.jpg` |
| `prone/` | `cobra-pose.jpg`, `locust-pose.jpg`, `sphinx-pose.jpg` |
| `standing/` | `mountain-pose.jpg`, `warrior-ii.jpg`, `triangle-pose.jpg` |
| `backbends/` | `bridge-pose.jpg`, `camel-pose.jpg`, `wheel-pose.jpg` |
| `forward-bends/` | `standing-forward-fold.jpg`, `seated-forward-fold.jpg`, `wide-legged-forward-fold.jpg` |
| `hip-openers/` | `butterfly-pose.jpg`, `pigeon-pose.jpg`, `low-lunge.jpg` |
| `seated/` | `easy-pose.jpg`, `staff-pose.jpg`, `hero-pose.jpg` |
| `twists/` | `seated-twist.jpg`, `supine-twist.jpg`, `revolved-chair.jpg` |
| `lateral-bends/` | `gate-pose.jpg`, `extended-side-angle.jpg`, `seated-side-bend.jpg` |

Tree Pose is already connected to `balancing/tree-pose.jpg`. Replace that file with another image using the same filename to update the card; no code change is needed.

For another pose, add its name and relative path to the `posePhotos` object in `asana-benefits.html`, for example:

```js
const posePhotos = {
  "Tree Pose": "images/asanas/balancing/tree-pose.jpg",
  "Dancer Pose": "images/asanas/balancing/dancer-pose.jpg"
};
```

Poses without a photo entry continue to show the built-in illustration.
