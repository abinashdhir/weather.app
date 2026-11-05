# Weather App

A small React + Vite weather app. Search any city and see its current temperature, humidity and wind speed, powered by the OpenWeatherMap Current Weather API. Bengaluru loads by default.

## Features

- City search with live conditions: temperature in °C, humidity, wind speed and the matching weather icon
- Default city on first load
- Basic error handling: an empty search and API errors (for example an unknown city) are reported to the user

## Tech stack

- React (hooks: `useState`, `useRef`, `useEffect`)
- Vite
- OpenWeatherMap Current Weather API
- ESLint

## Run locally

1. Install dependencies: `npm install`
2. Get a free API key at https://openweathermap.org/api
3. Copy `.env.example` to `.env` and set `VITE_APP_ID` to your key
4. Start the dev server: `npm run dev`

> Vite exposes `VITE_` variables to the browser bundle, so use a free-tier key and never commit your `.env` file (it is listed in `.gitignore`).

## Project structure

```
src/
  App.jsx                  app shell
  components/Weather.jsx   search bar, API call and weather display
  components/Weather.css   styles
```
