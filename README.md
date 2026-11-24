# Weather Dashboard

A weather app built with vanilla JavaScript and the free [Open-Meteo API](https://open-meteo.com) (no API key needed).

## Features

- Search any city; the Open-Meteo geocoding API returns up to 5 matches to pick from
- Current weather card: temperature, feels-like, humidity, wind speed, condition text and icon
- 7-day forecast with daily min/max temperatures
- Hourly temperature chart for today, drawn by hand on a `<canvas>` (no chart library)
- Remembers your last searched city in `localStorage` and loads it on startup
- Friendly error handling: unknown city, too-short query, and network failure

## What I practiced

- `fetch` with `async`/`await` against a real public API
- Combining two APIs (geocoding + forecast)
- Ignoring stale responses when the user searches again quickly (request counter)
- Canvas line-chart drawing with scaling and axis labels

## How to run it

Open `index.html` in a browser. An internet connection is needed for the weather data.

## Notes

A learning project. Weather data comes from Open-Meteo; the app only reads from it.
