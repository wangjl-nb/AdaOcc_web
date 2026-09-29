# Anonymous AdaOcc Project Page

This folder contains the static GitHub Pages-ready anonymous preview page for:

**AdaOcc: Adaptive 3D Occupancy Prediction for Embodied Tasks**

The page intentionally does **not** include author names, affiliations, contact details, code links, PDF downloads, or BibTeX entries.

## Files

```text
site/
├── index.html                    # Main project page with inline carousel interaction
├── CNAME                         # Custom GitHub Pages domain
├── .nojekyll                     # GitHub Pages static-site compatibility
├── README.md                     # This guide
└── static/
    ├── css/style.css             # Self-contained styling
    └── media/
        ├── README.md             # Media safety notes
        ├── videos/
        │   ├── main.mp4          # Browser-compatible main video
        │   └── poster.png        # Video poster frame
        ├── roll_pics/            # Image Overview carousel assets
        └── real_world/           # Real-world scenario section placeholders
```

## Safety rule: upload only `site/` contents

Do **not** upload the parent `projectpage_opus/` folder. It contains the paper PDF and downloaded example template files. Publish only the files inside `projectpage_opus/site/`.

## Current media

- Main video: `static/media/videos/main.mp4`
- Video poster: `static/media/videos/poster.png`
- Carousel images: `static/media/roll_pics/*.png`
- Real-world scenario images: `static/media/real_world/*.png`

PDF source figures from `roll_pics/` were rendered into PNG files for browser compatibility before publication. The original PDF sources are not part of this publish bundle.

## Preview locally

```bash
cd projectpage_opus/site
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Anonymous publishing checklist

Before publishing, confirm:

- [ ] `index.html` has no author names, contact details, homepages, or profile links.
- [ ] `index.html` has no affiliation, lab, company, or funding details.
- [ ] No code repository link is visible.
- [ ] No PDF download link is visible.
- [ ] No BibTeX entry with author data is visible.
- [ ] Media files do not contain watermarks, people, usernames, paths, or metadata that reveal identity.
- [ ] Only `site/` contents are pushed to the public repository.

## After anonymous review

After anonymous-review restrictions are lifted, `index.html` can be updated to add public paper, code, citation, author, and affiliation links.
