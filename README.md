# Sacred Sound & Spirit — Vercel Deploy

Static website. No build step required.

## Contents
```
index.html          → Landing page (home)
Legal.html          → Privacy / Terms / Policies
image-slot.js       → gallery helper script
vercel.json         → caching + clean URLs config
assets/             → backgrounds + logo (hero, philosophy, process, intake, logo-mortar)
fonts/              → Baskervville + Inter (self-hosted .ttf)
gallery/            → gallery-1…5.jpg
media/              → practitioner-intro.mp4
audio/              → client-testimonial.mp3
```

## Deploy — Option A: Drag & drop (easiest)
1. Go to https://vercel.com/new
2. Drag this entire `vercel-deploy` folder onto the page (or zip it first and upload).
3. Vercel auto-detects a static site — click **Deploy**. Done.

## Deploy — Option B: Vercel CLI
```bash
npm i -g vercel
cd vercel-deploy
vercel          # preview deploy
vercel --prod   # production deploy
```

## Deploy — Option C: Git
1. Push the contents of this folder to a GitHub repo.
2. In Vercel, **Add New → Project → Import** that repo.
3. Framework Preset: **Other**. Build command: *(none)*. Output dir: *(root)*. Deploy.

## Notes
- `index.html` is served at `/` automatically.
- Forms (intake + contact) submit via Formspree → form `xaqznnyj`. Submissions are
  emailed to the form owner; manage the recipient at https://formspree.io.
- To use a custom domain, add it under **Project → Settings → Domains** in Vercel.
