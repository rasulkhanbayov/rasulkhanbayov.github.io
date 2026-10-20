# rasulkhanbayov.github.io

Personal academic website: <https://rasulkhanbayov.github.io>

Plain HTML and CSS, no build step. GitHub Pages serves the files as they are.

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | Homepage: bio, news, research (with filter tabs) and experience |
| `papers/index.html` | Publications list |
| `papers/<slug>/index.html` | One page per paper: figure, summary, abstract, BibTeX |
| `cv/index.html` | HTML version of the CV |
| `data/Rasul_Khanbayov_CV.pdf` | PDF CV linked from every page |
| `cv_latex/Rasul_Khanbayov_CV.tex` | LaTeX source of the PDF CV |
| `styles.css` | All styling, including dark mode |
| `images/` | Profile photo, favicon and paper thumbnails (`images/thumbs/<slug>.jpg`) |

## Common edits

- **Add a news item:** copy a `<li>` inside `<div class="news">` in `index.html`.
- **Add a paper:** copy an `<article class="pub">` block in `index.html` and `papers/index.html`, copy one of the
  `papers/<slug>/` folders, and add a thumbnail to `images/thumbs/`. Use `data-type="peer"` or `data-type="preprint"`
  so the filter tabs work.
- **Update the CV:** edit `cv_latex/Rasul_Khanbayov_CV.tex` (on Overleaf, set the compiler to XeLaTeX or LuaLaTeX),
  then replace `data/Rasul_Khanbayov_CV.pdf` with the new PDF.

## Preview locally

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.
