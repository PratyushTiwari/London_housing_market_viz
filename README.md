# W12 Housing Market Interactive Visualization

Interactive map visualization of property transactions in the W12 (Shepherd's Bush) postcode district of London, covering 2005-2025.

## 🗺️ [View Live Map](https://pratyushtiwari.github.io/London_housing_market_viz/w12_market_map.html)

## Features

- **Interactive Map**: 587 postcode markers across W12 district
- **Multi-Level Analysis**:
  - Postcode level: Individual transaction histories with connected dot plots
  - Sector level: Aggregated statistics and trends for 4 sectors
  - District level: Overall W12 market analysis
- **Cohort Analysis**: Weighted average returns by purchase/sale period
- **Hover Interactions**: Dynamic highlighting of transaction histories
- **Area Highlighting**: Visual emphasis of sectors/districts on map

## Data Coverage

- **Time Period**: January 2005 - January 2025 (20 years)
- **Transactions**: 10,887 property sales
- **Properties**: 7,553 unique properties
- **Postcodes**: 587 postcodes across 4 sectors
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
open http://localhost:8000/w12_market_map.html
```

Note: A local server is required because the map loads popup files dynamically.

## File Structure

```
London_housing_market_viz/
├── w12_market_map.html    # Main interactive map (477 KB)
├── data/                   # JSON data files (3.7 MB)
│   ├── w12_postcodes.json
│   ├── w12_sectors.json
│   ├── w12_district.json
│   └── postcode_coords.json
└── popups/                 # Individual postcode popups (26 MB)
    ├── W12_0AA.html
    ├── W12_0AB.html
    └── ... (587 files)
```

## Market Insights (W12 District)

- **Average Price**: £641,228
- **Median Price**: £499,950
- **Price Growth**: From £250k (2005) to £655k (2024) median
- **Most Active Sector**: W12 9 (3,584 transactions)
- **Highest Appreciation**: Properties bought pre-2005, sold 2005 (~30% annual return)

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
