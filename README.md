# By Your Blood — site update

Drop these into your existing `living-words-site` folder, replacing where noted.

## New file
- `by-your-blood.html` — the song page (cover, chords download, on-page audio player, full lyrics).

## Replace existing files
- `index.html` — adds a sixth song card ("By Your Blood — A song of confession") to the home grid.
- `seasons.html` — adds By Your Blood as **The Still Centre**, a distinct block after the five seasons and before the Romans 8 close. It is deliberately NOT a sixth numbered season, per your framing of it as the ground the soul returns to.
- `styles.css` — adds one new block, `.still-centre`, for that Seasons feature. Everything else is unchanged.

## Add to your `assets/` folder
- `assets/cover-by-your-blood.png` — web cover (1400×1400; the 3000×3000 store master is separate).
- `assets/by-your-blood.mp3` — audio for the on-page player.
- `assets/by-your-blood-chords.pdf` — chord chart (see note below).

## Notes
- **No streaming buttons yet.** By Your Blood isn't live on Spotify/Apple (still in review with Symphonic), so the page launches with chords + audio only. There's an HTML comment in `by-your-blood.html` marking where the Spotify/Apple buttons go; add them once the release is live, matching the pattern in `find-me-here.html`.
- **Chord chart.** The PDF supplied is a raw Moises.ai export — it carries the Moises logo and a flat chord stream, and does NOT match your house-style charts (parchment, deep-green Cormorant heading, gold mono chords, James Thompson / Living Words Music footer). I've wired it in so the link works, but for consistency with the other five it should be rebuilt in the house style.
- **Scripture on the Seasons block** is Psalm 51:7 ("Wash me, and I shall be whiter than snow"), chosen to echo the chorus. Swap to 1 John 1:7 if you'd rather name the blood directly.
