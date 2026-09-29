# Anonymous media guide

Media in this folder is part of the publish-safe static site bundle. Do not place paper PDFs, source PDF figures, raw videos, author information, private paths, or identity-bearing files here.

## Current Image Overview carousel assets

The homepage carousel uses these PNG files under `static/media/roll_pics/`:

- `teaser.png`
- `pipeline.png`
- `device.png`
- `CPO.png`
- `occ_compare.png`
- `tartanground_adaptability.png`
- `open_vocabulary.png`
- `astar_plan.png`
- `nav_demo.png`
- `demo.png`

PDF source figures were rasterized to browser-safe PNG images. Generated and copied PNGs were re-saved without embedded PNG metadata.


## Current real-world scenario assets

The real-world section uses these PNG files under `static/media/real_world/`:

- `navigation-rgb.png`
- `navigation-depth.png`
- `navigation-occ.png`
- `manipulation-rgb.png`
- `manipulation-depth.png`
- `manipulation-occ.png`
- `mobile-manipulation-rgb.png`
- `mobile-manipulation-depth.png`
- `mobile-manipulation-occ.png`

These images are anonymous-safe placeholders for the current layout. Replace them with final matched RGB / geometry / occupancy captures when available.

## Main project video

The homepage video uses:

- `videos/main.mp4`
- `videos/poster.png`

The MP4 is transcoded to H.264 / yuv420p with the metadata atom moved to the beginning of the file for browser playback. The page preloads the video to improve compatibility with simple static-file mirrors that do not support byte-range seeking.

## Replacement checklist

Before replacing any media during anonymous review, check that frames, figure text, watermarks, filenames, and metadata do not reveal people, usernames, affiliations, institutions, local paths, or repository/account identities.
