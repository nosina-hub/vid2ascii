# vid2ascii ✨

> turn any video into real-time colored ascii art — right in your browser.

![made with love](https://img.shields.io/badge/made%20with-%F0%9F%A9%B7-black)
![no install](https://img.shields.io/badge/no%20install-just%20a%20html%20file-blueviolet)
![works offline](https://img.shields.io/badge/works-offline-success)

---

## what it does

vid2ascii takes a local video file and renders it frame-by-frame as **rgb colored ascii art** in a terminal-style display. no uploads, no servers, no dependencies — everything runs locally in your browser.

## features

- 🎞️ drag & drop any video (mp4, webm, mov, avi)
- 🌈 full rgb color per character, sampled directly from the video
- 🔤 multiple ascii ramps — simple, detailed, blocks, dots
- 🎚️ adjustable columns, fps cap, and volume
- ⚡ smooth real-time rendering via `requestAnimationFrame`
- 🔇 audio plays through with volume control
- 📦 single html file, zero dependencies

## how to use

1. open `index.html` in any modern browser
2. drag and drop a video file onto the drop zone
3. adjust cols, ramp style, and fps to your taste
4. hit **▶ play** and watch it go

## live demo

👉 [nosina-hub.github.io/vid2ascii](https://nosina-hub.github.io/vid2ascii)

## how it works

each video frame is drawn onto a hidden `<canvas>` scaled to the column count. pixel brightness maps to an ascii character from the chosen ramp, and the rgb value is applied as inline color — giving you full-color terminal art at whatever fps your machine can handle.

## customization

| control | what it does |
|--------|--------------|
| cols | width of the ascii output in characters |
| ramp | character set used for brightness mapping |
| fps cap | limits render rate to save cpu |
| vol | video audio volume |

---

made with 🩷 — a single html file that does something kinda cool
