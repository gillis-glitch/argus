# Argus — the world in real time 🌍

**Live → https://gillis-glitch.github.io/argus/**

Argus is a single-page, real-time situational dashboard: one map and five panels
showing what is happening right now — in the sky, on the ground, and in space.

## What it shows

- **Weather** — current conditions and next hours (Open-Meteo), with live rain
  radar and infrared satellite layers (RainViewer) on the map
- **Earthquakes** — every M ≥ 2 event in Italy from the last 7 days (INGV),
  plotted on the map with magnitude and distance
- **Flagged air traffic** — military aircraft, blocked/limited registrations
  (PIA/LADD), unidentified tracks and emergency squawks within 120 km,
  via the community ADS-B networks (adsb.lol / airplanes.live)
- **Space weather** — planetary Kp index, geomagnetic storm status and solar
  wind, straight from NOAA SWPC
- **Civil Protection alerts** — the official Italian hydro-meteorological
  criticality bulletin

An annunciator strip at the top summarises every domain at a glance:
green = quiet, amber = watch, red = alert.

## Features

- 🌐 **5 languages** (IT · EN · ES · RU · 中文), auto-detected from the browser —
  or forced with `?lang=en`
- 📍 **Any location**: search a place or use your position; panels and map follow
- 🔄 Self-refreshing (aircraft every 30 s, the rest at slower cadences)
- 🪶 **No server, no build, no framework**: one static HTML file. Your browser
  talks directly to the open data sources
- 🕵️ **No tracking, no cookies, no ads** — only anonymous, cookie-free visit
  counting (GoatCounter)

## Data sources

[Open-Meteo](https://open-meteo.com) ·
[RainViewer](https://www.rainviewer.com) ·
[INGV](https://terremoti.ingv.it) ·
[NOAA SWPC](https://www.swpc.noaa.gov) ·
[adsb.lol](https://adsb.lol) ·
[airplanes.live](https://airplanes.live) ·
[Protezione Civile](https://www.protezionecivile.gov.it) ·
maps © OpenStreetMap / CARTO · [Leaflet](https://leafletjs.com)

Some of these are volunteer-run networks — consider supporting them.

## Roadmap

- Cloudflare Worker proxy (cache + CORS bridge)
- Italian trains (live delays) and Bologna buses
- World mode: global earthquakes (USGS), wildfires (NASA FIRMS)
- Worldwide public transport via Transitland

---

## 🇮🇹 In breve

Argus è una "sala di controllo" in tempo reale in una sola pagina: meteo e radar
pioggia, terremoti INGV, traffico aereo segnalato (militari e voli schermati),
meteo spaziale NOAA e allerte della Protezione Civile, su un'unica mappa live.
Cinque lingue, nessun server, nessun tracciamento — solo conteggio visite
anonimo e senza cookie. Nato a Bologna, funziona ovunque: cerca la tua località
e Argus ti segue.
