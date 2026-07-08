# Playful app landing template — pure-CSS claymorphism

**Live demo → https://bswxyz.github.io/fable-clay/** · [How it was built](https://bswxyz.github.io/fable-clay/guide/)

> Candy-pastel clay shapes that bob, parallax and squish — a joyful product page with zero images.

A free, MIT-licensed website template. Good for: **consumer apps, kids' products, games, anything friendly**.
The demo brand ("CLAY") is fictional — every word and colour is meant to be replaced with yours.

## The signature technique

- Claymorphism recipe: outer drop shadow + inset light + inset press, all CSS
- Shapes bob on individual sine phases and parallax toward the cursor; poke = spring squish
- Squishy buttons and cards; rounded display type (Fredoka)

## Use this as your own site

This repo is a **template** — everything is plain HTML/CSS/JS with **relative paths**, so it
works under *any* repo name with zero configuration.

1. Click **Use this template → Create a new repository** (top of this page).
   **Name it whatever you like** — `my-site`, `portfolio`, anything.
2. In your new repo: **Settings → Pages → Build and deployment → Deploy from a branch**,
   then pick `main` / `/ (root)` and save. (CLI: see below.)
3. Wait ~1 minute. Your site is live at `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`.

<details>
<summary>Prefer the command line?</summary>

```bash
gh repo create my-site --template bswxyz/fable-clay --public --clone
cd my-site
gh api --method POST /repos/YOUR-USERNAME/my-site/pages \
  -f 'source[branch]=main' -f 'source[path]=/'
```
</details>

No build step, no dependencies to install — edit the files, push, done.
The only external requests are Google Fonts and (where used) pinned CDN copies of GSAP/three.js.

## Customize it

- Pastels: the candy palette is `:root` variables in `styles.css`
- Shapes: each hero shape is a positioned div — add/remove/resize freely
- Copy: headline, features and steps are plain HTML sections

The `/guide/` page documents the signature technique in depth (with code) — keep it, rewrite it,
or delete the folder entirely.

## Files

```
index.html        the page
styles.css        all styling (design tokens in :root at the top)
main.js           the signature effect + motion
guide/index.html  how-it-works write-up (optional — yours to keep or delete)
```

## Built-in quality

- Works with JS disabled or a CDN failure (content is never permanently hidden)
- Respects `prefers-reduced-motion`; keyboard focus styles throughout
- Canvas/WebGL feature-detected with graceful fallbacks; devicePixelRatio capped for performance
- Responsive at phone / tablet / desktop widths

## License & credit

[MIT](LICENSE) — free for personal and commercial use, no attribution required
(a link back is always appreciated). Originally designed & built by **Fable**
(Anthropic's Claude) as part of a 25-template collection:
**[the full gallery →](https://bswxyz.github.io/fable-showcase/)**
