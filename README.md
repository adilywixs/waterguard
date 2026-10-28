# 💧 WaterGuard

**Protect every drop.**

WaterGuard is a water-monitoring web app for schools, companies and public buildings. It compares actual water use with the normal pattern, finds unusual consumption that may mean a leak, shows where it happened, and estimates the water and money that could be lost.

> **Live demo:** _add your site link here_

## The problem

An organization gets a water bill every month, but the bill does not show **when** unusual use started or **where** it happened. A small leak can run for days without anyone noticing.

## How it works

1. **Data**: meter readings, a CSV file, or manual entry.
2. **Analyze**: compare the new reading with the baseline (the average of recent normal readings).
3. **Detect**: if the deviation is above the threshold, it is an anomaly.
4. **Alert**: a notification is created and the building turns red on the map.
5. **Act**: check the location, then mark the alert as resolved.

Example:

| | Value |
|---|---|
| Expected (baseline) | 80 m³ |
| Actual | 116 m³ |
| Deviation | +45% |
| Result | Possible leak / abnormal usage |

**Important:** WaterGuard does not see a broken pipe. It only finds unusual water use that may mean a leak. A person must always check on site.

## Features

- Landing page with the problem, solution and sources
- Sign up and sign in (demo, saved in the browser only)
- Dashboard: Overview, Water Monitoring, Alerts, Locations & Map, Analytics & Impact, Sources, AI Assistant, Settings
- Add a measurement or upload a CSV, then the anomaly check runs
- Notifications when an anomaly is found or an alert changes
- Schematic map with green, yellow and red locations
- Cost calculator (you enter your own local tariff)
- Assistant that explains the alerts in simple words
- Three languages: Русский, English, Қазақша

## CSV format

```csv
Date,Time,Location,Consumption
2026-10-23,03:00,Science Block,36
2026-10-23,03:00,Administration,29
2026-10-23,03:00,Sports Hall,64
```

Locations: Main Building, Sports Hall, Science Block, Administration.

## Demo account

- Email: `demo@waterguard.kz`
- Password: `demo123`

Or press **Use demo account** on the sign-in page.

## Run locally

No install needed. Download the project and open `index.html` in a browser.

## Honest notes

- All consumption numbers, savings and costs in the app are **demo data**.
- The tariff is a demo value. Real tariffs are different in each city.
- Accounts are saved in the browser (`localStorage`). This is **not** real authentication.
- The assistant uses ready answers based on the dashboard data. It is not a live AI model.
- The map is a schematic drawing, not a geographic map.

## Sources

External facts in the app show their source, date and reliability level. They come from Kazinform, 24KZ and the Bureau of National Statistics of Kazakhstan. Public statistics about water loss inside schools are limited, so WaterGuard is designed to help organizations collect this data. Open the **Sources & Methodology** page in the app for the full list.

## Tech

One HTML file with plain HTML, CSS and JavaScript. No backend and no database.

## Team

Zharassova Adilya 
