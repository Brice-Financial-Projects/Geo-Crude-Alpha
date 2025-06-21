# 🛢️ BSEE Oil Rig Location Data (U.S. Offshore)

The **Bureau of Safety and Environmental Enforcement (BSEE)** provides publicly accessible data on offshore oil and gas platforms, primarily focused on the **Gulf of Mexico**. This is a reliable, government-maintained source ideal for research, geospatial analysis, or integration into energy-related applications.

---

## 📍 Where to Access the Data

- **Data Portal**: [BSEE on Data.gov](https://catalog.data.gov/dataset?organization=bsee-gov)
- **Direct Dataset**: [Platforms in the Gulf of Mexico](https://data.boem.gov/Platform/Default.aspx)
- **Formats**: CSV, Excel, Shapefile, Geodatabase
- **Update Frequency**: Periodic (not real-time)

---

## 📦 Dataset Fields (Sample)

- `Platform_Name`: Name of the rig/platform
- `Latitude` / `Longitude`: Geographic coordinates
- `Operator_Name`: Company responsible for the rig
- `Water_Depth`: Depth of water beneath the platform
- `Installation_Date`: When the platform was installed
- `Platform_Status`: Active, Decommissioned, etc.
- `Region`: Location code (e.g., Gulf of Mexico)

---

## 🧰 Suggested Tools for Exploration

| Tool        | Purpose                         |
|-------------|----------------------------------|
| `pandas`    | Load and analyze tabular data   |
| `geopandas` | Handle shapefiles or geodata    |
| `folium`    | Create interactive maps         |
| `duckdb`    | Fast SQL querying on local files|
| `Streamlit` | Build quick dashboard apps      |
| `FastAPI`   | Wrap data in an API if needed   |

---

## 🧪 Sample Code Snippet (Python)

```python
import pandas as pd
import folium

# Load the CSV file
df = pd.read_csv('platform_locations.csv')

# Create a map centered in the Gulf of Mexico
m = folium.Map(location=[27.5, -90.0], zoom_start=6)

# Add rig markers
for _, row in df.iterrows():
    folium.CircleMarker(
        location=[row['Latitude'], row['Longitude']],
        radius=3,
        popup=row['Platform_Name']
    ).add_to(m)

# Save the map
m.save("gulf_platforms_map.html")
