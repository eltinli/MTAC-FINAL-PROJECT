# Data Folder Metadata

This document describes the contents and sources of the files in the `data/` folder of the MTAC Fire Simulation project.

---

## 📁 Files and Descriptions

### 1. `newforecast_output_2030_clean.xlsx`
- **Description**: Forecasted barangay-level population for the year 2030.
- **Source**: Derived from Philippine census data (PSA, 1990–2020).
- **Notes**: Generated using linear and regression models in the forecasting notebook.

### 2. `merged_barangay_centroids_44.csv`
- **Description**: Latitude and longitude of centroids for 44 barangays in Iligan City.
- **Source**: Calculated from OSM-extracted polygons.
- **Projection**: EPSG:4326 (WGS84).
- **Use**: Used for distance and ETA calculations.

### 3. `IliganData_Stations.xlsx`
- **Description**: List of existing fire stations with their coordinates.
- **Source**: Digitized from Iligan City LGU maps and public documents.
- **Use**: Defines land-based response nodes in the simulation.

### 4. `full_iligan_roads_buffer/edges.shp` (+ `.dbf`, `.shx`, `.prj`)
- **Description**: Shapefile representing road edges with buffer zones.
- **Source**: Extracted from OpenStreetMap using OSMnx, with manual preprocessing.
- **Use**: Used for routing, travel distance, and ETA analysis.

---

## 📌 Notes

- All geographic files are in EPSG:4326 unless otherwise noted.
- Ensure all shapefile components (`.shp`, `.dbf`, `.shx`, `.prj`) are kept together.
- File paths in the simulation are accessed using Python's `os.path.join("data", filename)` for reproducibility.

---

## 📚 Citation Format

If using the data or this model in a derived work, please cite:

> MTAC Fire Simulation: A Population-Driven Spatial Optimization of Air Response in Iligan City, 2025.
