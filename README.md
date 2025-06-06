# AI-Based Biodiversity Hotspot Mapping

This project applies machine learning techniques to map biodiversity hotspots by analyzing environmental variables and species occurrence data. It enables the identification of areas rich in species to support conservation planning and ecological research.

## Project Overview

The workflow includes:
- Loading environmental raster layers (NDVI, elevation, temperature).
- Extracting raster values at species richness occurrence points.
- Training a Random Forest model to predict species richness.
- Generating a spatially continuous biodiversity hotspot map.
- Exporting prediction results for further analysis.

## Files Generated

- `biodiversity_hotspots.tif` — GeoTIFF raster of predicted biodiversity richness.
- `Biodiversity_Hotspot_Predictions.xlsx` — Excel file containing:
  - **Latitude**
  - **Longitude**
  - **Predicted Species Richness**

## How to Use

1. **Prepare the Data**:
   - Collect and align raster layers (e.g., NDVI, elevation, temperature).
   - Gather species richness point data (shapefile with richness values).

2. **Install Required Libraries**:
```bash
pip install numpy pandas geopandas rasterio scikit-learn matplotlib openpyxl
```

3. **Run the Script**:
   - Load raster layers and species points.
   - Train the Random Forest model.
   - Generate the biodiversity hotspot map.
   - Export the predictions to Excel.

4. **Review the Outputs**:
   - Open `biodiversity_hotspots.tif` in GIS software.
   - Open `Biodiversity_Hotspot_Predictions.xlsx` in Excel to review predictions.

## Key Features

- **Random Forest Model**: Predicts species richness based on environmental variables.
- **Spatial Predictions**: Generates continuous maps for visualizing biodiversity patterns.
- **Export Options**: Outputs results in both raster and tabular formats.

## License

This project is licensed under the MIT License.

## Author

Ebiere
