# Skyline

A single-file weather app where you scrub through the day and watch the sky change.

Vanilla HTML, CSS and JavaScript. No dependencies, no build step.

## Features

- **Live forecasts** from [Open-Meteo](https://open-meteo.com/) (no API key), with a demo-data fallback when offline.
- **Time scrubber**: drag the chart or slider, or use the arrow keys, to move through the day. A canvas sky morphs in real time: gradient by sun elevation and weather, sun and moon arc, stars, drifting clouds, rain, snow and lightning.
- **Hourly temperature chart** and a **7-day forecast** with range bars. Click a day to view it.
- **City search** with autocomplete, geolocation (with an approximate network-based fallback), and saved cities.
- **°C / °F** toggle. Settings are stored in `localStorage`.
- **Accessible**: semantic landmarks, ARIA live regions, keyboard control, focus rings, and `prefers-reduced-motion` support.

## Run

Open `index.html` in a modern browser. For precise GPS location, serve it over HTTPS or `http://localhost`, for example:

```
python -m http.server 8000
```

Then visit http://localhost:8000.

## Notes

- The default city is Stockholm, Sweden.
- Weather data is fetched from Open-Meteo. The approximate location fallback uses ipwho.is.
