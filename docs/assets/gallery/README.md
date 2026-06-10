# Gallery assets

Drop CFD images and videos here, then reference them from `docs/gallery.md`.

## Adding an image

1. Add the file, e.g. `vortex-shedding.jpg`.
2. In `docs/gallery.md`, add inside `.gallery-grid` (no blank lines between items):

```html
<div class="gallery-item" data-type="image" data-src="assets/gallery/vortex-shedding.jpg" data-caption="Vortex shedding behind a cylinder" tabindex="0" role="button">
    <img src="assets/gallery/vortex-shedding.jpg" alt="Vortex shedding behind a cylinder" loading="lazy">
    <div class="gallery-caption">Vortex shedding behind a cylinder</div>
</div>
```

## Adding a video

1. Add the file, e.g. `jet-flow.mp4` (MP4/H.264 recommended for browser compatibility).
2. In `docs/gallery.md`, add inside `.gallery-grid`:

```html
<div class="gallery-item" data-type="video" data-src="assets/gallery/jet-flow.mp4" data-caption="Turbulent jet flow simulation" tabindex="0" role="button">
    <video src="assets/gallery/jet-flow.mp4" muted loop playsinline preload="metadata"></video>
    <div class="gallery-play-icon">
        <svg viewBox="0 0 24 24" fill="currentColor"><path d="M8 5v14l11-7z"></path></svg>
    </div>
    <div class="gallery-caption">Turbulent jet flow simulation</div>
</div>
```

## Tips

- Keep videos short and compressed (a few MB) — they autoplay muted on hover.
- The placeholder card (`gallery-placeholder`) can be removed once real items are added.
- Captions appear on hover/focus and in the lightbox when an item is clicked.
