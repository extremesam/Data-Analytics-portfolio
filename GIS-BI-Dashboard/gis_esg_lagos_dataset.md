# 🗺️ GIS + ESG Analytics Dataset — Lagos Urban Dashboard

A geo-referenced ESG dataset covering all 20 Lagos LGAs, built for spatial heat analysis, green space mapping, vulnerability indexing, and executive ESG reporting. Compatible with QGIS, ArcGIS, and Power BI Map.

---

## 📁 Workbook Structure (4 Sheets)

| Sheet | Purpose |
|-------|---------|
| **GIS Spatial Data** | 299 geo-referenced data points across all 20 LGAs — plug directly into Power BI Map or QGIS |
| **LGA Summary** | Aggregated metrics per LGA with Lat/Lon for choropleth maps |
| **Land Use Distribution** | Breakdown of heat, green cover & vulnerability by land use type |
| **KPI Summary** | Executive ESG dashboard snapshot |

---

## 🗂️ Column Reference (17 Columns)

| Group | Fields |
|-------|--------|
| **Location** | Record ID, LGA, Latitude, Longitude |
| **Heat Analysis** | Surface Temp Index (°C), Heat Zone (color-coded) |
| **Green Space** | Green Cover (%), NDVI Index, Green Space Access |
| **Population** | Population Density (per km²), Population Exposure Index |
| **Vulnerability** | Vulnerability Score, Vulnerability Class, Income Proxy Score |
| **ESG** | ESG Score, Land Use Type, Area km² |

---

## 📊 Key Dataset Findings

| Metric | Value |
|--------|-------|
| 🌡️ Avg Surface Temp | 38.6°C |
| 🔴 Extreme Heat Zones | 17.4% of all data points |
| 🌿 Avg Green Cover | 30.1% — unevenly distributed (Mushin/Agege lowest) |
| ⚠️ Critical Vulnerability | 26.1% of all data points |
| 📊 Avg ESG Score | 41.2 / 100 — significant improvement headroom |

---

## 📺 Power BI Visualization Mapping

| Visual | Source Sheet | Fields |
|--------|-------------|--------|
| Heat Map | GIS Spatial Data | Lat, Lon + Surface Temp Index (bubble/heat layer) |
| Green Space Map | GIS Spatial Data | Lat, Lon + Green Cover % or NDVI Index |
| Vulnerability Index Map | LGA Summary | Lat, Lon + Vulnerability Class (choropleth) |
| Land Use Classification | Land Use Distribution | Pie / donut or treemap |
| Population vs Heat Exposure | GIS Spatial Data | Pop Density vs Exposure Index (scatter plot) |

---

## 🎨 Color Coding

| Column | Coding |
|--------|--------|
| Heat Zone | 🔴 Extreme · 🟡 Moderate · 🟢 Low |
| Vulnerability Class | 🔴 Critical · 🟡 High · 🟢 Low |

> Both columns are pre-color-coded in Excel for instant visual scanning — no conditional formatting setup required.

---

## 🛠️ GIS Compatibility

| Tool | How to Use |
|------|-----------|
| **Power BI** | Load GIS Spatial Data sheet → Map visual → Lat + Lon fields → add measure as bubble size or color saturation |
| **QGIS** | Export sheet to CSV → Add Delimited Text Layer → set Lat/Lon as geometry fields |
| **ArcGIS** | Import CSV → XY Table to Point → project in WGS84 (EPSG:4326) |

---

## 🚀 Use Cases

- Urban heat island analysis and climate risk mapping
- Green space equity and NDVI spatial visualization
- Community vulnerability and social exposure indexing
- ESG scoring dashboards for Lagos LGAs
- Land use classification and urban planning reporting
