# ianturner.github.io

Personal academic site — GitHub Pages.

## One-time setup

1. Create a GitHub account with the username you want in the URL (e.g. `ianturner`).
2. Create a **new public repository** named exactly `USERNAME.github.io`.
   The repo name *must* match your username, or the site won't publish at the root URL.
3. Upload the contents of this folder to the repo (drag-and-drop into the web
   uploader is fine — no git required).
4. Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
5. Wait ~1 minute. Site is live at `https://USERNAME.github.io`.

## Before you publish — edit these

In `index.html`:
- `YOUR.EMAIL@example.com` → your email (appears twice)
- `YOUR-USERNAME` in the footer GitHub link
- ORCID / Google Scholar links, or delete them

## Folder layout

```
index.html          the whole site (one file, no build step)
talks/              conference slides as PDF
cv/                 put ian-turner-cv.pdf here
```

## Adding a new talk

1. Export the deck to PDF (File → Save As → PDF in PowerPoint).
2. Drop it in `talks/` with a filename like `turner-2026-topic-venue.pdf`.
3. Copy an existing `<article class="item">` block in `index.html`, change the text
   and the link. Commit.

## Keeping the repo small

- Always publish **PDF, never .pptx**. The three decks here went from 8.3 MB to 1.9 MB.
- If a PDF is still over ~5 MB, the cause is uncompressed images. Re-export with
  "Minimum size" / "Optimize for web," or in Acrobat use Save As → Reduced Size PDF.
- Audio and video do not belong in the repo. Host those on Zenodo and link out.
- Hard limits, for reference: 100 MB per file, 1 GB recommended per repo,
  1 GB per published Pages site.

## Audio

`audio/` holds three MP3 clips pulled out of the Quechua deck (they were embedded
in the .pptx all along). Re-encoded to mono 64 kbps — 199 KB for all three.

**Before publishing these, confirm your participant consented to public release
of the recordings**, not just to their use in a conference talk. If consent covers
presentation only, either pull the clips or replace them with waveform/spectrogram
images, which raise no such issue.
