# [ESP32 Serial Monitor](https://esp32-monitor-rho.vercel.app)

[https://esp32-monitor-rho.vercel.app](https://esp32-monitor-rho.vercel.app)

A browser-based serial monitor for ESP32 (and any USB serial device). No install required — just open the site, plug in your board, and click Connect.

It is compatible with any USB serial device including: Arduino Unos, Arduino Nanos, ESP32s, and more.

Built with the [Web Serial API](https://developer.chrome.com/docs/capabilities/serial) — works entirely in the browser, no backend needed.

**Made by [Kayan Shah](https://github.com/KayanShah)**

---

## Features

- Auto-detects baud rate (configurable: 9600 → 921600)
- Colour-coded output (errors, warnings, success, info, debug)
- Timestamped lines with millisecond precision
- Send data back to ESP32
- Export full session log as `.txt`
- Auto-scroll with pause-on-scroll
- Line count + byte counter

## Browser Support

Requires **Chrome 89+** or **Edge 89+** on desktop. Firefox and Safari do not support the Web Serial API.

## Deploy to Vercel

1. Fork or clone this repo to your GitHub account
2. Go to [vercel.com](https://vercel.com) → New Project → Import your repo
3. Vercel auto-detects the static site — just click **Deploy**
4. Done. Share the URL.

## Local Development

Just open `index.html` in Chrome — it's a single static file with no dependencies.

```bash
# Or serve locally with any static server:
npx serve .
```

## Usage

1. Plug your ESP32 into USB
2. Open the site in Chrome/Edge
3. Select your baud rate (default: 115200)
4. Click **Connect** and choose your COM/tty port
5. Serial output streams in real time
