# Studio site — where to put photos & video covers

Drop your files into these folders. Then tell me (or edit `studio.html`) to show them.

```
img/studio/
├── product/        → product photography (jewelry, e-commerce, catalog, hero shots)
├── content/        → brand / lifestyle / food content
├── video-covers/   → cover images for videos (if not using a YouTube thumbnail)
└── about/          → your personal / on-set photo  →  portrait.jpg
```

## Naming
Use short, lowercase, no-spaces names, e.g. `gold-necklace-01.jpg`, `cafe-latte.jpg`.
JPG for photos. Aim for the long edge ~2000px and keep each file under ~500 KB
(I can batch-compress them for you — just ask).

## Your personal photo (the one you wanted to change)
Replace **`about/portrait.jpg`** with the photo you want. Keep the same filename and
it shows up automatically — no code change needed.
Tip for a brand site: an "on set / with camera" candid often reads better than a
formal headshot. It says *working creative* instead of *LinkedIn profile*.

## Adding a new work tile to the gallery
Each frame in the Work section is one block in `studio.html`. Copy this, change the
`src`, `data-full`, `data-cat` (product / content / video), and the caption text:

```html
<div class="g-item" data-cat="product" data-full="img/studio/product/gold-necklace-01.jpg">
  <img loading="lazy" src="img/studio/product/gold-necklace-01.jpg" alt="Gold necklace">
  <div class="cap"><div class="k">Product</div><div class="t">Your caption here</div></div>
</div>
```
Add `wide` or `tall` to the class (e.g. `class="g-item wide"`) to make a frame feature-sized.
Or just drop files in the folders and I'll wire them up.
