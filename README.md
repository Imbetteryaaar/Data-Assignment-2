# Australia's Wild Quarter

A data visualisation of Australia's national parks and protected natural areas,
built for **FIT2179 Data Visualisation 2**, Monash University, Semester 1 2026.

The project is a single, scrollable web page that tells one story with **13
Vega-Lite visualisations**, including **two maps** (a choropleth and a
proportional-symbol map).

## Repository contents

```
index.html                     The complete web page (HTML + CSS in one file)
data/
  australia-states.json         Simplified GeoJSON of the states/territories (map geometry)
charts/
  01-protected-area-map.json    Choropleth map — % of land protected by state
  02-protected-growth-lines.json  Multi-line — land vs sea protection over time
  03-terrestrial-area-target.json Area chart — growth toward the 30%-by-2030 target
  04-protection-drivers.json    Stacked bar — Indigenous Protected Areas vs other
  05-largest-parks-bar.json     Horizontal bar — 10 largest national parks
  06-largest-parks-map.json     Proportional-symbol map — those 10 parks located
  07-oldest-parks-timeline.json Dot-plot timeline — 10 oldest national parks
  08-nsw-visits-column.json     Column chart — NSW park visits over time
  09-visits-donut.json          Donut — domestic vs international visits
  10-top-parks-lollipop.json    Lollipop — most-visited NSW parks
  11-icon-parks-slope.json      Slope chart — Uluru vs Kakadu visitors, 2023→2024
  12-threatened-species-bar.json Bar — threatened species (plants vs animals)
  13-establishment-decades.json Histogram — parks established per decade
sketch/                         Put your hand-drawn sketch PDF here
WRITEUP-500-words.md            Text for the Moodle submission form
SKETCH-GUIDE.md                 Instructions for drawing the required sketch by hand
_gen.py                         Build script that generated the chart specs (reference)
```

Every Vega-Lite specification in `charts/` is plain JSON, formatted for human
readability. The page loads each chart from its `.json` file at run time.


## Data sources

- ABS — *Protected areas* (2025), based on CAPAD —
  <https://www.abs.gov.au/statistics/measuring-what-matters/measuring-what-matters-themes-and-indicators/sustainable/protected-areas>
- DCCEEW — *Collaborative Australian Protected Areas Database (CAPAD)* —
  <https://www.dcceew.gov.au/environment/land/nrs/science/capad>
- NSW National Parks & Wildlife Service — record park-visitation media release (2025)
- Parks Australia & state park agencies — park areas, history and visitor data
- DCCEEW — *Threatened species under the EPBC Act* —
  <https://www.dcceew.gov.au/environment/biodiversity/threatened/species>
- State boundary geometry — `world-geojson` (Natural Earth derived), simplified
  by the author.

## Author & licence

Created by **Gaurav** — Monash University, FIT2179 Data Visualisation 2,
Semester 1 2026. Published May 2026.

