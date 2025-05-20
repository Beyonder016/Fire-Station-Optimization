# 🚒 Fire Station Optimization using the DC Building Dataset

This project optimizes the location of fire stations in Washington, D.C. by identifying underserved regions and proposing optimal new station placements using geospatial analysis and machine learning.

## 📍 Visuals
| Map Type               | Live Link |
|------------------------|-----------|
| 🟧 Building Density     | [View Map](https://beyonder016.github.io/Fire-Station-Optimization/interactive/building_density_map.html) |
| 🟥 Existing Stations    | [View Map](https://beyonder016.github.io/Fire-Station-Optimization/interactive/existing_fire_stations_map.html) |
| 🔵 Proposed Stations    | [View Map](https://beyonder016.github.io/Fire-Station-Optimization/interactive/proposed_fire_stations_map.html) |

## 📌 Objective
- Minimize response time for fire emergencies.
- Identify high-risk or underserved zones.
- Suggest new fire station locations using clustering.

## 🧰 Tech Stack
- Python, Pandas, GeoPandas
- H3 (Hexagonal spatial indexing)
- Scikit-learn (KMeans clustering)
- Folium (Interactive Maps)
- Geopy (Distance calculation)

## 📊 Methodology
1. **Load and clean building data**
2. **Convert to H3 hexagons** (Resolution 9)
3. **Overlay fire station data**
4. **Calculate underserved zones** (>1 km away)
5. **Cluster underserved hexes** using KMeans
6. **Suggest locations** and visualize results

## 📁 Files
- `fire_df.csv`, `Fire_Stations.csv` – Raw fire station data
- `underserved_df.csv` – Computed underserved regions
- `kmeans_firestation_model.pkl` – Saved clustering model
- `DC_Emergency_Optimization_Map.html` – Interactive final map
- `fire_station_analysis.ipynb` – Full notebook (Colab-ready)

## 📜 License
MIT

---
