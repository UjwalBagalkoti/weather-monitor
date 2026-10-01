# Weather Monitor

A live weather monitoring dashboard — real-time conditions, an hourly forecast chart, and a 7-day outlook, styled like a meteorological instrument console.

Created by **UjwalBagalkoti**.

## Live Demo
https://weather-monitor-vert.vercel.app/

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
   git clone https://github.com/UjwalBagalkoti/weather-monitor.git
   cd weather-monitor
   ```
2. Open `index.html` directly in your browser, or serve it locally:
   ```bash
   python3 -m http.server 8000
   ```
   then visit `http://localhost:8000`.

## Deploy on Vercel

1. Import the repository into Vercel.
2. Use the default static-site settings.
3. Deploy. No build command is required.

The current production deployment is linked above.

> **Note:** Open-Meteo's API must be reachable from wherever you view the page. It works from a plain browser tab or GitHub Pages; it will not work inside a sandboxed preview panel that restricts outbound network requests.

## Tech

- Vanilla HTML/CSS/JS — no framework, no build tooling
- [Chart.js](https://www.chartjs.org/) for the hourly temperature chart
- [Open-Meteo](https://open-meteo.com/) for weather and geocoding data

