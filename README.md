# Happy Birthday: A Personalised Birthday Website

A single-page, mobile-first birthday surprise built with plain HTML, CSS and JavaScript. No frameworks, no build step, no backend.

**Live demo:** https://Swati06-maurya.github.io/Happy-Birthday/

## What it does

- **Sealed-envelope intro:** a wax-seal envelope with a 3D flap animation. Tap the seal and the flap opens and the letter slides out.
- **Living background:** the sky changes from sunrise to day to dusk to a starry night as you scroll. Clouds, hills and a swaying wheat field sit behind the content.
- **Procedural wheat field:** every stalk, ear and grain is drawn on HTML canvas in three depth layers. Nothing is an image.
- **Interactive sections:** flip cards, collectable wish-stars, a shayari section and a diary-style finale with a photo.
- **Confetti finale:** a canvas confetti burst, plus a replay button.
- **Optional extras:** birthday countdown chip and a real-photo background, both switched on from the config.

## Tech used

- HTML5 and CSS3 (custom properties, 3D transforms, clip-path, keyframe animations)
- Vanilla JavaScript (DOM, IntersectionObserver, scroll-driven theming)
- Canvas 2D (wheat field and confetti)
- SVG filters (wax seal texture, clouds)
- Google Fonts (Playfair Display, Poppins, Kalam, Tiro Devanagari Hindi)

## Project structure

```
Happy-Birthday/
├── index.html    # the whole site: markup, styles and script
└── README.md
```

## Customise it

All text and options live in one `CONFIG` object at the top of the `<script>` block in `index.html`: name, village, birthday date, cards, wishes, shayari, final message and photo. Change the values and refresh the page.

| Option | What it does |
| --- | --- |
| `birthday: "MM-DD"` | Shows a countdown on the first screen, and fires confetti on the day |
| `showAge` / `age` | Shows an age chip |
| `photo` | Photo shown in the diary (a file path or a base64 data URI) |
| `fieldPhoto` | A real photo used as the sky and field background |

## Run locally

Open `index.html` in any modern browser. An internet connection is only needed for the Google Fonts.

## Deploy with GitHub Pages

1. Push the repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `main` branch and `/ (root)`, then click **Save**.
5. After a minute or two the site is live at `https://<username>.github.io/<repository>/`.

## What I learned

- Building a layered, animated scene with canvas and SVG instead of image assets
- 3D CSS transforms for the envelope-flap interaction
- Driving page theme and background from scroll position
- Designing mobile-first, with reduced-motion support

## License

Made as a personal gift. Feel free to reuse the code as a template for your own surprise.