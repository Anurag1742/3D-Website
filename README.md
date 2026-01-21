# 3D Website (Spline + AOS Landing Page)

A modern, responsive 3D landing page built with plain **HTML + CSS**, featuring a live **Spline** 3D scene and smooth **AOS (Animate On Scroll)** entrance animations.

![Preview](thumbnail.png)

## Features

- **Interactive 3D model** embedded via `spline-viewer`
- **Scroll/entrance animations** via AOS attributes (`data-aos`, `data-aos-duration`, etc.)
- **Dark, modern UI** with a gradient glow background
- **Responsive layout** (desktop + tablet + mobile breakpoints)
- **No build step**: runs directly in the browser

## Tech Stack

- HTML5
- CSS3 (flexbox, gradients, media queries)
- [Spline Viewer](https://spline.design/) (loaded from CDN)
- [AOS](https://michalsnik.github.io/aos/) (loaded from CDN)

## Project Structure

```
.
├── index.html      # Markup + Spline/AOS integration
├── style.css       # Styling + responsive rules
├── gradient.png    # Background gradient image
├── thumbnail.png   # README preview image
├── youtube.png     # Optional asset (if used for promo/links)
├── LICENSE
└── README.md
```

## Run Locally

### Option 1: Open directly
1. Download/clone the repository.
2. Open `index.html` in your browser.

### Option 2 (Recommended): VS Code Live Server
1. Install the **Live Server** extension.
2. Right-click `index.html` → **Open with Live Server**.

## Customize

### Change the 3D scene
In `index.html`, replace the Spline scene URL:

```html
<spline-viewer url="https://prod.spline.design/YR58cjeB9dBOiQFK/scene.splinecode"></spline-viewer>
```

To use your own scene:
1. Export/Publish your project from Spline.
2. Copy the hosted `.splinecode` URL.
3. Paste it into the `url` attribute.

### Update text/branding
- Logo text: `MCODE`
- Headline: `EMAIL FOR DEVELOPERS`
- Buttons/links: update the anchors in the `.buttons` section

### Adjust animation timing
Animations are controlled via AOS attributes such as:
- `data-aos="fade-down"`
- `data-aos-duration="1500"`
- `data-aos-delay="300"`

You can tweak duration/delay per element to get the motion you want.

### Change colors & layout
Most styling lives in `style.css`, including:
- Background glow (`.layer-blur`) and gradient element (`.image-gardient`)
- Layout and spacing (`header`, `.content`, `.buttons`)
- Responsive behavior (`@media (max-width: 1300px)` and `@media (max-width: 768px)`)

## Notes

- This page loads Spline and AOS from CDNs, so an internet connection is required.
- If the 3D model doesn’t appear, check that:
	- the Spline URL is reachable
	- your browser allows loading external scripts

## License

MIT — see `LICENSE`.