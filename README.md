# YT MultiView

Watch four YouTube videos at once in a 2×2 grid, with synced playback.

**Live app:** https://gooodufo.github.io/yt-multiview/

## Features

- 2×2 grid of independent YouTube players, landscape-first layout
- Search YouTube in each tile (needs a free YouTube Data API v3 key — add it in ⚙ Settings; stored only in your browser)
- Or paste a YouTube link / video ID into any tile (no key needed)
- **▶ All** – play every loaded video together
- **⏸ All** – pause everything
- **↻ Sync** – restart all videos from 0:00 at the same moment
- Installable as a home-screen app (PWA); locks to landscape on Android

## Add to your phone's home screen

- **iPhone:** open the link in Safari → Share → *Add to Home Screen* (rotate the phone for landscape)
- **Android:** open the link in Chrome → menu → *Add to Home screen* (installs locked to landscape)

## Getting a YouTube API key (for search)

1. Enable the [YouTube Data API v3](https://console.cloud.google.com/apis/library/youtube.googleapis.com) in Google Cloud (free tier is plenty).
2. Create an [API key](https://console.cloud.google.com/apis/credentials) under Credentials.
3. Paste it into the app's ⚙ Settings.
