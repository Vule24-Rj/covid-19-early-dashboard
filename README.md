# COVID-19 Early Outbreak Dashboard (Feb-March 2020)

## How to Run
1. Keep `covid-19.json` and `index.html` in same folder
2. Open `index.html` in browser OR: `python -m http.server 8000`
3. No login needed

## Calculations
- Daily new cases = confirmed[today] - confirmed[yesterday], 0 if negative
- Active cases = confirmed - deaths - recoveries
- First day daily = that day's confirmed

## Chart Library
Chart.js - lightweight, responsive, supports line + bar, easy vanilla JS. Chosen over D3.js (too complex) and Plotly (heavy).

## Handling Missing Dates
Filter skips missing dates gracefully, chart shows only available dates. FALLBACK data included if JSON fails to load.

## Testing Evidence
- China peak Feb
- Italy rapid growth March
- South Africa first case March 5
- Daily new matches known figures

## Insights
China containment after Feb, Italy becomes epicenter March, SA late start.
