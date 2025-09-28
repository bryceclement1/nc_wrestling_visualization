# nc_wrestling_visualization

An interactive map visualization of **North Carolina 2A Wrestling (2021–2025)** results.<br/>
Built with [Leaflet.js](https://leafletjs.com/) and custom JSON/GeoJSON data, it allows users to explore county-level wrestling performance with filters for **year** and **weight class**.

[Visualization Link](https://bryceclement1.github.io/nc_wrestling_visualization/)

---

## 🌍 Features
- Interactive **Leaflet map** centered on North Carolina.
- **County-level shading** based on total wrestling performance scores.
- Dynamic **filters** for:
  - Year (2021–2025, or all years combined)
  - Weight class
- Tooltips and popups showing:
  - Total score
  - 1st, 2nd, and 3rd placers
  - Most Outstanding Wrestlers (MOW)
- Responsive design with map legend and county labels.

---

## 📂 Project Structure
.
├── index.html # Main entry point (loads map & controls)
├── main.js # Leaflet logic, map rendering, filters
├── style.css # Styling for map, controls, tooltips, legend
├── nc_county_scores_by_year_and_weight.json # County scores data
├── National_Atlas_County_Boundaries_(USGS).geojson # County boundary shapes
└── NCWrestling.csv # Source dataset (optional reference)


📊 Data Notes
North Carolina state tournament data for 2021-2025 scraped from [Track Wrestle](https://www.trackwrestling.com/TWHome.jsp?loadBalanced=true).  
Scores are stored by county → year → weight class in nc_county_scores_by_year_and_weight.json.

Each record includes:

first, second, third, mow, and aggregated score.

GeoJSON boundaries come from the National Atlas County Boundaries (USGS) dataset.

🛠️ Built With
Leaflet.js for maps

HTML5 / CSS3 / JavaScript

GeoJSON for county shapes

Custom JSON for wrestling scores
