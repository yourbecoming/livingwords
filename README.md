# Living Words Music — website

A static site (plain HTML + CSS). No build step, no framework. Deploys to Vercel in minutes.

## Files
```
index.html                     Home
only-you-king-jesus.html       Song page
find-me-here.html              Song page
about.html                     About / bio
styles.css                     Shared styles (Living Words identity)
assets/
  symbol.svg                   Logo mark (used as favicon + in header/footer)
  avatar.svg                   Full avatar (spare, if needed)
  cover-only-you.png           Cover art
  cover-find-me-here.png       Cover art
  only-you-king-jesus-chords.pdf
  find-me-here-chords.pdf
```

## Deploy to Vercel (using your existing account)

**Option A — drag & drop (fastest)**
1. Go to vercel.com → Add New → Project.
2. If it asks for a Git repo, choose "Deploy without Git" / use the Vercel CLI, OR put this folder in a new GitHub repo and import it.
3. Easiest no-Git route: install the CLI once (`npm i -g vercel`), then from inside this folder run `vercel` and follow the prompts. Run `vercel --prod` to publish.

**Option B — GitHub (recommended for easy future edits)**
1. Create a new GitHub repo, upload these files.
2. In Vercel → Add New → Project → import that repo.
3. Framework preset: **Other** (it's static). Build command: none. Output directory: leave as root (`.`).
4. Deploy.

## Connect your domain (livingwordsmusic.org)
1. In the Vercel project → Settings → Domains → add `livingwordsmusic.org` (and `www.livingwordsmusic.org`).
2. Vercel shows you the DNS records to set. At your domain registrar, add those records (usually an A record + a CNAME for www, or Vercel's nameservers).
3. HTTPS is automatic once DNS propagates (minutes to a couple of hours).

## Before you publish — two edits
1. **Streaming links.** In `only-you-king-jesus.html` and `find-me-here.html`, find the lines marked
   `<!-- Replace href="#" ... -->` and paste the live Spotify and Apple Music URLs once the releases are live.
   Until then the buttons sit harmlessly on `#`.
2. **CCLI number** (optional, later). Once registered, you can add the CCLI number near the chord download on each song page.

## Adding a future song
Copy `find-me-here.html` to a new file (e.g. `walk-with-me.html`), swap the title, cover image, lyrics, and chord PDF, then add a matching `<a class="song-card">` block to the Songs grid in `index.html`. That's it.

## Notes
- Fonts (Cormorant Garamond, EB Garamond) load from Google Fonts, so the real typeface renders everywhere — no font issues.
- The whole identity (green, gold, mark) lives in `styles.css`; change a colour once there and it updates site-wide.
