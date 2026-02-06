# London Housing Market Interactive Visualization

Interactive map visualization of property transactions across 13 North and West London postcode districts, covering 2005-2025.

## 🗺️ [View Live Map](https://pratyushtiwari.github.io/London_housing_market_viz/london_housing_market_map.html)

## Features

- **Interactive Map**: 9,230+ postcode markers across 13 districts
- **Multi-Level Analysis**:
  - Postcode level: Individual transaction histories with connected dot plots
  - Sector level: Aggregated statistics and trends for 76 sectors
  - District level: Analysis for each of 13 districts
- **Cohort Analysis**: Weighted average returns by purchase/sale period
- **Hover Interactions**: Dynamic highlighting of transaction histories
- **Area Highlighting**: Visual emphasis of sectors/districts on map

## Data Coverage

- **Time Period**: January 2005 - January 2025 (20 years)
- **Districts**: 13 postcode districts (W12, NW2, NW10, W9, W6, SW6, NW5, N7, N19, N6, N16, N2, N3)
- **Transactions**: 165,000+ property sales
- **Properties**: 115,000+ unique properties
- **Postcodes**: 11,000+ postcodes across 76 sectors
- **Repeat Sales**: Detailed analysis of properties sold multiple times

## Technical Details

- Built with [Folium](https://python-visualization.github.io/folium/) (Leaflet.js)
- Interactive charts powered by [Plotly.js](https://plotly.com/javascript/)
- Data from [HM Land Registry Price Paid Data](https://www.gov.uk/government/statistical-data-sets/price-paid-data-downloads)
- Geocoding via [postcodes.io](https://postcodes.io/)

## Usage

### Online (Recommended)
Simply visit the GitHub Pages link above - no setup required!

### Local Viewing
```bash
# Clone this repository
git clone https://github.com/PratyushTiwari/London_housing_market_viz.git
cd London_housing_market_viz

# Start local server
python3 -m http.server 8000

# Open in browser
open http://localhost:8000/london_housing_market_map.html
```

Note: A local server is required because the map loads popup files dynamically.

## File Structure

```
London_housing_market_viz/
├── london_housing_market_map.html  # Main interactive map (7.1 MB)
├── data/                           # JSON data files (65 MB)
│   ├── all_postcodes.json
│   ├── all_sectors.json
│   ├── all_districts.json
│   └── postcode_coords.json
└── popups/                         # Individual postcode popups (404 MB)
    ├── W12_0AA.html
    ├── NW2_1AA.html
    └── ... (11,111 files)
```

## Market Insights (Across All Districts)

- **District Price Range**: From £397k (NW10) to £931k (SW6) average
- **Most Transactions**: SW6 (Fulham) with 25,489 sales
- **Largest District**: N2 (East Finchley) with 1,939 postcodes
- **Repeat Sales**: 50-60% of transactions across most districts
- **Typical Holding Period**: 6-6.5 years median
- **Annual Appreciation**: 4.8-5.7% median across districts

## Data Sources & Attribution

Contains HM Land Registry data © Crown copyright and database right 2025. This data is licensed under the [Open Government Licence v3.0](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

Postcode coordinates from [postcodes.io](https://postcodes.io/) (Open Government Licence).

## Related Research

This visualization is part of a broader research project analyzing London housing market dynamics. For the full analysis pipeline and methodology, see the [main research repository](https://github.com/PratyushTiwari/London_housing_market) (private).

## License

- **Code**: MIT License
- **Data**: Open Government Licence v3.0

---

**Created with**: Python, Folium, Plotly, and Claude
**Last Updated**: February 2025
