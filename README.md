# Portfolio & Résumé Website

A clean, classic, single-page portfolio + résumé site built with plain
**HTML, CSS, and JavaScript** — no build step, no dependencies. Just edit the
files and publish on GitHub Pages.

🔗 **Live (after you enable Pages):** `https://thatnhattran.github.io/Resume/`

---

## 📁 Project structure

```
Resume/
├── index.html        ← all the page content (edit your details here)
├── css/style.css     ← all styling + theme colours + print/PDF layout
├── js/main.js        ← menu, scroll animations, "Download Résumé"
├── favicon.svg       ← the little tab icon (your initials)
├── assets/           ← put your photo.jpg / resume.pdf here (optional)
└── .nojekyll         ← tells GitHub Pages to serve the files as-is
```

---

## ✏️ How to personalise it

The name and contact details are currently **placeholders** so nothing private
is published by accident. Search `index.html` for the comments marked
`EDIT ME` — each one points to something to change:

| What to change | Where |
|---|---|
| Your name | `Your Name` (appears in nav, hero, footer, page title) |
| Your initials (monogram) | `YN` in `index.html` **and** in `favicon.svg` |
| Email | `your.email@example.com` |
| GitHub link | `github.com/yourusername` |
| LinkedIn link | `linkedin.com/in/yourprofile` |
| Phone (optional) | not shown by default — add it in the hero contacts list |
| Professional title / summary | the `hero__title` and `hero__summary` lines |

> Tip: use your editor's **Find & Replace** to swap `Your Name` everywhere at once.

**Change the colours:** open `css/style.css` and edit the variables at the very
top (`:root { … }`) — `--navy` (primary) and `--accent` (gold) re-skin the
whole site.

**Add a photo or PDF:** see `assets/README.md`.

---

## 🚀 Publish on GitHub Pages

1. Push this code to your repository (the `main` branch).
2. On GitHub, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Set **Branch** to `main` and folder to **`/ (root)`**, then **Save**.
5. Wait ~1 minute, then visit **`https://thatnhattran.github.io/Resume/`**.

That's it — every time you push to `main`, the live site updates automatically.

> The files for this site currently live on the `claude/beautiful-shannon-85j8b3`
> branch. Merge that branch into `main` (or open a pull request) before enabling
> Pages, or point Pages at that branch directly in step 4.

---

## 👀 Preview locally (optional)

You can just double-click `index.html` to open it in a browser. For everything
to behave exactly like the live site, serve it from a folder:

```bash
# Python 3 (no install needed on most machines)
python3 -m http.server 8000
# then open http://localhost:8000
```

---

## 📄 Download / print as PDF

The **Download Résumé** button uses a dedicated print stylesheet to turn the
page into a clean, single-column résumé — choose *Save as PDF* in the print
dialog. (Prefer a real PDF file? See `assets/README.md`.)
