# AdaOcc Project Page

Static GitHub Pages site for **AdaOcc: Adaptive 3D Occupancy Prediction for Embodied Tasks** (NeurIPS 2026).

**Live site:** <https://wangjl-nb.github.io/AdaOcc_web/>

## Files

```text
.
├── index.html                    # Main project page with inline carousel interaction
├── .nojekyll                     # GitHub Pages static-site compatibility
├── README.md                     # This guide
└── static/
    ├── css/style.css             # Self-contained styling
    └── media/
        ├── README.md             # Media notes
        ├── videos/
        │   ├── main.mp4          # Browser-compatible main video
        │   └── poster.png        # Video poster frame
        ├── roll_pics/            # Image Overview carousel assets
        └── real_world/           # Real-world scenario assets
```

## Current media

- Main video: `static/media/videos/main.mp4`
- Video poster: `static/media/videos/poster.png`
- Carousel images: `static/media/roll_pics/*.png`
- Real-world scenario assets: `static/media/real_world/*`

PDF source figures from `roll_pics/` were rendered into PNG files for browser compatibility. The original PDF sources are not part of this bundle.

Media totals roughly 79 MB, of which about 53 MB is video. GitHub Pages has a soft bandwidth limit of 100 GB per month, so consider offloading or re-encoding the videos if the page starts drawing heavy traffic.

## Preview locally

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Deployment

The site is published from the `main` branch root via GitHub Pages (`Deploy from a branch` → `main` → `/`). Push to `main` and the site rebuilds automatically. There is no build step: the repository contains the served files directly.

## Custom domain

No custom domain is currently configured; the site is served from the default `*.github.io` address. To attach one, set it under **Settings → Pages → Custom domain** and create the matching DNS records at your registrar:

- Apex domain (`example.com`): `A` records to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- Subdomain (`www.example.com`): `CNAME` record to `wangjl-nb.github.io` (without the repository name)

A given custom domain can be attached to only one GitHub Pages site across all of GitHub.

## Related repositories

- Code, data preparation, and reproduction docs: <https://github.com/wangjl-nb/AdaOcc>
- Released checkpoints: <https://huggingface.co/wjldragon/AdaOcc>
