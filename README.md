# AI Image Generator

A free, client-side AI image generator. Type a prompt, pick a model, and get AI-generated images instantly — right in your browser. No login, no install, no backend.

## Features

- **Text-to-image generation** — enter a prompt and generate images using Google's Gemini / Imagen 3.0 models
- **Prompt suggestions** — built-in suggestion gallery to spark ideas and fill the prompt box in one click
- **Image preview modal** — full-size preview of generated results
- **Generation history** — recently generated images saved in a thumbnail grid during the session
- **One-click download** — save any generated image to your device
- **Dark modern UI** — Tailwind CSS glassmorphism design with sparkle effects and responsive layout

## Tech Stack

- HTML, CSS, JavaScript (single-file app, no build step)
- Tailwind CSS via CDN
- Google Generative Language API (Gemini 2.0 Flash / Imagen 3.0)

## Quick Start

This is a plain static site — no build or install needed.

1. Open `index.html` in any modern browser (or serve the folder with any static server).
2. Paste your **Google Gemini API key** (get a free one at [Google AI Studio](https://aistudio.google.com/)) when prompted — the key stays in your browser and is never stored anywhere else.
3. Type a prompt, hit generate, and download your image.

### Serve locally

```bash
npx serve .
# or
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Project Structure

```
AI-Image-Generator/
└── index.html      # entire app: markup, styles (Tailwind CDN), and JS
```

## API Key / Env Vars

- `GEMINI_API_KEY` — required at runtime, entered in the browser; the app calls `generativelanguage.googleapis.com` directly from client-side JavaScript. No server, no proxy, no key is ever committed to this repo.

## Deploy

Static site — deploy anywhere that serves static files. Currently live on GitHub Pages.

## License

Free to use. **Built by [Girish Lade](https://ladestack.in)**.
