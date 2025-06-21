# 🛢️ Onshore Oil Rig Location Data (U.S.)

Unlike offshore platforms, onshore oil rig location data is **fragmented**, often hidden behind state-level agencies or commercial paywalls. However, there are both **public and commercial sources** available depending on your budget, use case, and level of detail required.

---

## 📚 Summary of Available Sources

| Source                      | Type       | Notes |
|-----------------------------|------------|-------|
| **Baker Hughes Rig Count**  | Public     | Weekly rig count by region/state, no exact locations |
| **Enverus RigData**         | Commercial | Most complete rig-level data: GPS, contractor, spud date |
| **State Oil & Gas Agencies**| Public     | Permit-level data (location, depth, status) by state |
| **FracFocus**               | Public     | Data on hydraulic fracturing wells with location info |
| **EIA (U.S. Energy Info)**  | Public     | Aggregated county-level rig/well data |
| **Kayrros / Planet Labs**   | Commercial | Satellite-based rig tracking and oilfield analytics |

---

## 🧭 Public Data Sources (U.S. Onshore)

### 1. 🔢 Baker Hughes Rig Count
- **Website**: [https://rigcount.bakerhughes.com/](https://rigcount.bakerhughes.com/)
- **Focus**: National rig totals by basin or state
- **Limitations**: No lat/lon or rig-specific data
- **Use Case**: Market trend analysis, economic modeling

---

### 2. 🏛️ State-Level Oil & Gas Agencies

Each state maintains its own oil and gas regulatory database, often with well permit maps and reports.

| State     | Resource |
|-----------|----------|
| **Texas** | [Texas RRC GIS Viewer](https://gis.rrc.texas.gov/GISViewer/) |
| **North Dakota** | [NDIC Oil & Gas Division](https://www.dmr.nd.gov/oilgas/) |
| **Colorado** | [COGCC Data Portal](https://cogcc.state.co.us/) |

You can extract well or rig info by:
- Downloading shapefiles / spatial layers
- Scraping permit PDFs or CSVs
- Converting PLSS / township-range info to GPS coordinates

---

### 3. 💧 FracFocus
- **Website**: [https://fracfocus.org/](https://fracfocus.org/)
- **Focus**: Hydraulic fracturing well disclosures
- **Data**: Operator, API number, location, water volumes
- **Limitations**: Focused on fracking sites, not all rigs

---

## 💰 Commercial Source: Enverus RigData

If you need **accurate**, **GPS-based**, and **up-to-date** rig location data, Enverus is the go-to solution.

- **Website**: [https://www.enverus.com/solutions/rigdata/](https://www.enverus.com/solutions/rigdata/)
- **Data Includes**: Rig coordinates, contractor, spud date, depth, basin, permit link
- **API Access**: Available for integration
- **Use Case**: Energy trading, logistics, production planning, forecasting

---

## 🛰️ Advanced: Satellite-Based Services

### Kayrros, Planet Labs, Ursa Space
These services use satellite imagery + AI to track:
- Rig movements
- Frac crew activity
- Well completions
- Methane flares / emissions

Use case: Advanced modeling, hedge fund tools, ESG monitoring

> ⚠️ These tools are **expensive** but extremely powerful when combined with financial models or supply chain risk tools.

---

## ✅ Recommendations by Use Case

| Goal | Recommended Source |
|------|--------------------|
| Free rig trend tracking | Baker Hughes |
| Individual well permits | State Oil & Gas Portals |
| Full rig GPS coordinates | Enverus RigData (paid) |
| Environmental impact studies | FracFocus + Satellite |
| Commodity alpha/signal engine | Hybrid (Enverus + permits + satellite) |

---

## 🛠️ Tool Suggestions for Integration

- `pandas` for tabular analysis
- `geopandas` for shapefiles and geodata
- `duckdb` for efficient querying
- `folium` / `leaflet.js` for mapping
- `FastAPI` or `Flask` to wrap data in a backend
- `Streamlit` or `Dash` for building dashboards

---

## 📌 Notes

- Onshore rig data is **not centralized** like offshore.
- For real-time or mobile rig tracking, **commercial APIs are essential**.
- Public data is rich but requires **scraping, parsing, and cleanup** for production use.

