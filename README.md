# Weather Monitor

A live weather monitoring dashboard — real-time conditions, an hourly forecast chart, and a 7-day outlook, styled like a meteorological instrument console.

Created by **UjwalBagalkoti**.

## Features

- Live current conditions: temperature, feels-like, humidity, pressure, UV index, wind speed and direction
- Rotating wind-direction compass gauge
- 24-hour temperature chart
- 7-day forecast strip
- City search with autocomplete, or use your device's location
- Auto-refreshes every 5 minutes
- No API key, no backend, no build step — a single static HTML file

Data is pulled live from the free [Open-Meteo](https://open-meteo.com/) API.

## Getting started

This is a single static HTML file with no dependencies to install.

1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
   cd <your-repo>
   ```
2. Open `index.html` directly in your browser, or serve it locally:
   ```bash
   python3 -m http.server 8000
   ```
   then visit `http://localhost:8000`.

## Deploy with GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Save. Your app will be live at `https://<your-username>.github.io/<your-repo>/`.

> **Note:** Open-Meteo's API must be reachable from wherever you view the page. It works from a plain browser tab or GitHub Pages; it will not work inside a sandboxed preview panel that restricts outbound network requests.

## Tech

- Vanilla HTML/CSS/JS — no framework, no build tooling
- [Chart.js](https://www.chartjs.org/) for the hourly temperature chart
- [Open-Meteo](https://open-meteo.com/) for weather and geocoding data

## License

MIT — see [LICENSE](LICENSE).
