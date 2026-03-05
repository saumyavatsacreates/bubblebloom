# Bubble Bloom — Vercel Deployment

## Files
- `index.html` — the complete game (single file, zero dependencies)
- `vercel.json` — routing, caching, and security headers

## Deploy via GitHub → Vercel

1. Push this folder's contents to the **root** of your GitHub repo
2. Go to [vercel.com](https://vercel.com) → Add New Project
3. Import your GitHub repo
4. Settings:
   - **Framework Preset:** Other
   - **Root Directory:** `./` (or whichever folder contains index.html)
   - **Build Command:** *(leave blank)*
   - **Output Directory:** `./`
5. Click Deploy — live in ~30 seconds

Every push to `main` auto-deploys. No build step needed.

## Custom Domain
Vercel Dashboard → your project → Settings → Domains → Add domain
