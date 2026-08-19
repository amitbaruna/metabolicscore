# Metabolic Score — Landing Page (Rebuilt)

This is a plain static rebuild of the original Next.js export, since the
export you had was missing its entire `_next/static/` folder (JS, CSS,
fonts) and could never have worked as deployed. This version has no
build step — it's just `index.html` + images + Tailwind loaded from a
CDN — so it will work on **any** static host (Cloudflare Pages, Netlify,
GitHub Pages, Vercel, or even opened as a local file).

## What to check
- **Case study photos** (`/cases/case1.jpg` – `case8.jpg`): I matched
  these from the 16 before/after photos in your original export,
  prioritizing correct gender for the two perimenopause cases. Open
  each one against its card copy on the page and swap any that don't
  match the story — just replace the file, same name, same folder.
- **Font**: the original used Vercel's "Geist" font, which isn't
  available on this environment. I substituted Google's "Inter" —
  visually very close (same geometric/modern style), but not pixel-identical.
- **Unused photos**: `ba9.png` – `ba16.png` and the other unmatched
  originals aren't included here — let me know if you want them added
  as extra case studies or a gallery.

## Deploying
Push this whole folder to a **new** GitHub repo (the old
`amitbaruna/metabolicscore` repo doesn't exist), then connect it to
Cloudflare Pages / Netlify / Vercel, or enable GitHub Pages on it —
no build command needed, just "static site, serve as-is."
