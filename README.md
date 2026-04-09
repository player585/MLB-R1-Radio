# MLB R1 RADIO

A Rabbit R1 native web app for streaming live MLB radio broadcasts.

## Overview

This app is designed specifically for the **Rabbit R1** device (240×282px display), styled with the signature Rabbit Orange (`#ff4e00`). It fetches today's MLB games from [free-sportsradio.com](https://www.free-sportsradio.com/scores/mlb) via a CORS proxy and presents each game with a **Listen Now** button that expands to show stream links.

## Features

- 🟠 Rabbit R1 native dimensions (240×282px)
- 🎛️ Scroll wheel support (Arrow keys / Volume keys in R1 WebView)
- 📻 Live MLB game detection via CORS proxy (AllOrigins)
- 🔗 Direct links to game broadcasts and team station pages
- 📱 Touch-friendly tap-to-expand station selector

## Usage

Open `index.html` directly on your Rabbit R1 browser or deploy via GitHub Pages.

## How It Works

1. On load, fetches `https://www.free-sportsradio.com/scores/mlb` through the AllOrigins CORS proxy
2. Parses the HTML response for "Listen Now" links
3. Renders a game card for each found broadcast
4. Tapping **Listen Now** expands station options to open the stream

## Hardware Notes

- Built for Rabbit R1 Android WebView (240×282 viewport)
- Scroll wheel mapped to `ArrowUp`/`ArrowDown` and `AudioVolumeUp`/`AudioVolumeDown`
- No external dependencies — pure vanilla HTML/CSS/JS

## License

MIT
