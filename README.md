# rayeedaabir.github.io

Source for my personal research page: **https://rayeedaabir.github.io**

It is a single static page (plain HTML and CSS, no JavaScript, no tracking, no build step) hosted with GitHub Pages. Every push to `main` goes live within a few minutes.

## Folder layout

```
rayeedaabir.github.io/
├── index.html        the whole page: content, structure, link-preview tags
├── style.css         all styling (colours and fonts are defined at the top)
├── cv.pdf            CV, linked from the header
├── README.md         this file (not shown on the site)
├── LICENSE           licence terms (code vs. content)
├── img/
│   ├── portrait.webp           720x720 photo, top of the page
│   ├── fusion.webp             fusion project, bright-light strip
│   ├── fusion-qualitative.webp fusion project, nine methods on one frame
│   ├── decolor.webp            decolorization project, comparison grid
│   ├── decolor-demo.webp       still shown before the decolorization video plays
│   ├── continual.webp          continual-learning project, pipeline figure
│   └── og.png                  1200x630 link-preview card (email, LinkedIn, Slack)
├── video/
│   ├── fusion-demo.mp4         (optional fallback: fusion-demo.gif)
│   └── decolor-demo.mp4        (optional fallback: decolor-demo.gif)
└── fonts/
    ├── atkinson-hyperlegible-latin-400-normal.woff2
    ├── atkinson-hyperlegible-latin-400-italic.woff2
    └── atkinson-hyperlegible-latin-700-normal.woff2
```

Each of `img/`, `video/` and `fonts/` has a `README.txt` with the exact file names and sizes. The page still loads if a file is missing: images show their alt text, and the font falls back to the visitor's default sans-serif.

## Before the first publish

Anything still unfinished is highlighted in yellow on the page (the `todo` class). To find every one, search the repository for `class="todo"`. Fill each in, then delete `class="todo"` from that element so the highlight disappears. Open spots at the time of writing:

- [ ] Cureus paper link (when the paper is online)
- [ ] arXiv preprint links (only if the preprints are posted; otherwise delete those lines)
- [ ] Video notes under the two demos (add the `.mp4` files, then delete the notes)
- [ ] `img/portrait.webp`, `img/fusion.webp`, `img/continual.webp`, `cv.pdf` and the three font files

## How to update the site

On GitHub, no software needed:

1. Open the file in the repository and click the pencil icon to edit it, or use **Add file → Upload files** for images, videos and the CV.
2. Write a short commit message and click **Commit changes**.
3. Wait 1 to 3 minutes, then reload the page. Progress shows under the **Actions** tab.

On your computer: edit the files, then open `index.html` in a browser to preview. No server is needed.

### Update checklist

When something changes, work down this list:

- [ ] **New paper accepted or published:** change its tag in "Selected work" (`Manuscript` → `Accepted` → `Published`), add the paper link, and update the matching line in "Publications".
- [ ] **New project:** copy an existing `<article class="project">` block, add its figure to `img/` with descriptive alt text, and keep the claims to numbers you can show.
- [ ] **New CV:** replace `cv.pdf` (keep the same file name so the link keeps working).
- [ ] **Status line:** update the "Applying for…" sentence in the header and the `description` and `og:description` text in `<head>` if the wording changes.
- [ ] **Experience or education:** edit the dated rows at the bottom of `index.html`.
- [ ] **Footer date:** change "Last updated" at the bottom of `index.html`.
- [ ] **New photos or figures:** export as `.webp`, about 1400 px wide, under roughly 300 KB.
- [ ] **Link preview:** if the headline or name changed, regenerate `img/og.png`, then refresh the cached preview with LinkedIn's Post Inspector.
- [ ] **Check:** open the live page in a private window, check it at phone width, and click every link.

### Size limits to know

GitHub's web upload accepts files up to 25 MB, and any single file over 100 MB is blocked. Keep each demo video under 25 MB and the whole repository well under 1 GB.

## Licence and credits

- **Code** (`index.html` markup and `style.css`) is released under the MIT licence, see [LICENSE](LICENSE).
- **Content is not covered by that licence.** All text, photos, figures, demo videos and the CV are © 2026 Rayeed Aabir Ahsan, all rights reserved. Figures from published or submitted papers may also be subject to the publisher's terms.
- **Font:** [Atkinson Hyperlegible](https://brailleinstitute.org/freefont) by the Braille Institute, under the SIL Open Font License 1.1. It keeps its own licence.
- **Profile icons** (Google Scholar, GitHub, ORCID, LinkedIn) are trademarks of their owners and are used only to link to my profiles there.

## Contact

rayeed.ahsan@northsouth.edu
