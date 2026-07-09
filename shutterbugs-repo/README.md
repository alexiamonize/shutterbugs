# Shutterbugs 📸

A bilingual (English / Russian) single-page website for a kids' photography school offering age-tiered courses.

## Features
- **EN / RU language toggle** — full-page translation via a lightweight `data-i18n` dictionary, no frameworks
- Three course tracks by age (6–8, 9–12, 13–16) with curriculum, pricing, and duration
- Free trial class signup form with client-side validation (bilingual error/success messages)
- Photography-themed design: viewfinder brackets, EXIF-style labels, polaroid cards, animated film strip
- Responsive to mobile, keyboard-accessible, respects `prefers-reduced-motion`

## Structure
Single self-contained file: `index.html` (HTML + CSS + JS). Google Fonts is the only external dependency.

## Run locally
Open `index.html` in any browser, or serve it:
```bash
python3 -m http.server 8000
```

## Deploy
Works out of the box with GitHub Pages: Settings → Pages → deploy from `main` branch root.

## Customizing translations
All copy lives in the `I18N` object at the bottom of `index.html`, keyed by language (`en`, `ru`). Edit strings there; elements pick them up via `data-i18n` attributes.
