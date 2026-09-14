# Alok Bhandari — Portfolio

Single-file static portfolio (clone of supash-dev style, magenta studio theme). No build step — deploy the folder as-is on Vercel.

## Deploy (Vercel)

1. Push this folder to a GitHub repo, then **Vercel → Add New → Project → Import** the repo. Framework preset: **Other**. No build command, output = root.
2. Or: `npx vercel` inside this folder.

## Structure

- `index.html` — the whole site (inline CSS/JS)
- `assets/videos/` — compressed 720p showreel + 4 edits
- `assets/images/` — 8 gallery pieces (full, ≤1600px)
- `assets/thumbs/` — thumbnails + video posters
- `assets/Alok-Bhandari-Resume.pdf` — **YOU ADD THIS** (resume button 404s until then)

## Before going live — search `TODO(ALOK)` in index.html

1. Contact links: email, phone, Behance, Instagram (`#` placeholders now)
2. `INBOX` const in the `<script>` (brief-form destination)
3. Portrait: save as `assets/images/portrait.jpg`, swap into FIG.01
4. Stats numbers, skill levels, experience entries, testimonial quotes
5. Project titles (EDIT 02–05 have working titles), canonical URL in `<head>`

## Swapping media later

- Videos: replace files in `assets/videos/` (H.264 mp4, ≤720p, run through `-movflags +faststart`), match the existing filenames or update the `<source>` + `poster` paths.
- Gallery: full image → `assets/images/`, 800px thumb → `assets/thumbs/thumb-<same-name>`, update the button's `data-full`, `img src`, caption.
- Originals (full-res) live only in the Drive folder — never committed, keeps deploys fast.
