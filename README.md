# YT MultiView

Watch four YouTube videos at once in a 2×2 grid, with synced playback.

**Live app:** https://gooodufo.github.io/yt-multiview/

## Features

- 2×2 grid of independent YouTube players, landscape-first layout
- **⊞ layout toggle** – cycle between 2×2 (4 tiles), 2×3 (6), 2×4 (8), and 2×5 (10). Extra columns sit side-by-side in landscape and stack as rows in portrait. Shrinking the grid closes the hidden tiles to free decoding/network resources
- Search YouTube in each tile (needs a free YouTube Data API v3 key — add it in ⚙ Settings; stored only in your browser)
- Or paste a YouTube link / video ID into any tile (no key needed)
- **Custom skip** – every playing tile has «/» buttons that jump back/forward by an adjustable amount; set any number of seconds in ⚙ Settings, decimals included (e.g. 6.76)
- **Per-tile loop** – tap a tile's ⟳ to loop it from exactly where it is: it plays for that tile's loop length, jumps back to that point, and repeats until you tap ⟳ again. Every tile has its own length, shown right on its ⟳ button — long-press ⟳ to change just that tile (decimals fine, e.g. 11.5s), and it sticks across reloads. ⚙ Settings holds the default that new tiles start from
- **Colourblindness filters** – each tile's 🎨 button cycles through four effects applied to that video: protanopia, deuteranopia, tritanopia, and achromatopsia (grayscale), then back to off
- **▶ All** – play every loaded video together
- **⏸ All** – pause everything
- **↻ Sync** – restart all videos from 0:00 at the same moment
- Installable as a home-screen app (PWA); locks to landscape on Android

## Sound on iPhone / iPad

iOS only allows **one video with sound** to play at a time — starting a second
unmuted video would pause the first (that's a WebKit rule, not something the
app can lift). So on iOS all tiles play muted except one: the first video you
load gets the sound, and every playing tile shows a speaker button (🔊/🔇) —
tap it to move the sound to that tile, or tap the active one to mute
everything.

## Add to your phone's home screen

- **iPhone:** open the link in Safari → Share → *Add to Home Screen* (rotate the phone for landscape)
- **Android:** open the link in Chrome → menu → *Add to Home screen* (installs locked to landscape)

## Getting a YouTube API key (for search)

1. Enable the [YouTube Data API v3](https://console.cloud.google.com/apis/library/youtube.googleapis.com) in Google Cloud (free tier is plenty).
2. Create an [API key](https://console.cloud.google.com/apis/credentials) under Credentials.
3. Paste it into the app's ⚙ Settings.
