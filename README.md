# Behold Again International Foundation — website

Static site, no build step. Ready for Vercel.

## Pages
- `/` — main website (`index.html`)
- `/profile` — organisation profile, printable to A4 (`profile/index.html`)
- `/BAIF_Organisation_Profile.pdf` — downloadable profile
- `404.html` — shown for unknown links

## Deploy on Vercel

**Option A — GitHub (recommended, auto-updates on every change)**
1. Create a new GitHub repository and upload the contents of this folder (not the folder itself) to it.
2. In Vercel, choose **Add New → Project**, import the repository.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Click **Deploy**.

**Option B — Vercel CLI**
```
npm i -g vercel
cd baif-site
vercel --prod
```

## Before going live
- Replace the placeholder email `info@beholdagain.org` everywhere it appears (use find-and-replace in `index.html` and `profile/index.html`).
- Confirm the office location ("Kampala, Uganda").
- After connecting a custom domain, change `og:image` in both pages to the full URL, e.g. `https://yourdomain.org/assets/og-image.png`, so link previews show the image on WhatsApp and social media.
- If you edit the profile, re-export the PDF: open `/profile`, click **Print**, choose **Save as PDF**, A4, margins **None**, background graphics **on**, and replace `BAIF_Organisation_Profile.pdf`.
