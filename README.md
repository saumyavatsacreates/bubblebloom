# Bubble Bloom 🫧

A browser-based mindfulness game. Pop 36 bubble-wrap domes to reveal hidden art.
Peel off the plastic sheet to complete the puzzle.

## Deploy to Netlify in 30 seconds

### Option A — Drag & Drop (fastest)
1. Go to [netlify.com](https://netlify.com) and sign in
2. Click **"Add new site"** → **"Deploy manually"**
3. Drag this entire `bubble-bloom-netlify` folder onto the upload area
4. Done — Netlify gives you a live URL instantly

### Option B — GitHub (auto-deploy on every push)
1. Push this folder to a GitHub repository
2. In Netlify: **"Add new site"** → **"Import an existing project"** → connect GitHub
3. Set **Publish directory** to `.` (dot) — no build command needed
4. Click **Deploy** — every `git push` auto-deploys

### Option C — Netlify CLI
```bash
npm install -g netlify-cli
cd bubble-bloom-netlify
netlify deploy --prod --dir .
```

## Custom Domain
Netlify dashboard → **Domain settings** → **Add custom domain**
HTTPS is automatic via Let's Encrypt (free).

## Files
| File | Purpose |
|------|---------|
| `index.html` | The complete game — single self-contained file |
| `netlify.toml` | Security headers, cache rules, build config |
| `_redirects` | SPA fallback routing |

## No build step needed
This is pure HTML/CSS/JS. No Node, no npm install, no webpack.
Everything — game logic, 16 procedural artworks, Web Audio synthesis,
animations — is inside `index.html`.
