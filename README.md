# F1 Dashboard - My Personal Pit Wall

I've been building this dashboard to keep track of everything F1 - race results, standings, calendar, and news - all in one place. It pulls data from the Ergast API (the go-to free F1 data source) and displays it in a clean, grid-based layout.

## What's On The Dashboard

The main section shows upcoming race countdown with the circuit name and date. Below that, there are three columns:
- Driver standings showing top 10 with their team and points
- Constructor standings with all 10 teams
- Race points from the last race

The calendar section has all the races for the season with dates and venue details. There's also a news section that pulls in F1 articles.

## How It Works

Just open index.html in any browser. The page automatically fetches data from:
- Ergast API for standings and race results
- OpenF1 for live timing during races

Driver and constructor data refresh every couple of minutes to keep things current.

## Customizing Team Names

I mapped the short team names to their full 2025 branding. If you want to change them, look for the `teamFullNames` section in the JavaScript - you can update the mapping there.

## Tech Stuff

It's all vanilla HTML, CSS, and JavaScript. No frameworks, just straightforward front-end work. The API calls are standard fetch requests that run on page load and on timers.
