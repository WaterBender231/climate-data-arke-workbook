# Unit 01 — Data Handling: From Raw DWD Rasters to Analysis-Ready Data

## Learning objectives

After this unit, you will be able to:

- Download gridded climate data from the German Weather Service (DWD) in bulk
- Extract and organize large climate raster archives
- Convert raster formats (ASCII Grid → GeoTIFF)
- Inspect and handle coordinate reference systems (CRS)
- Reproject rasters to a common spatial reference
- Clip rasters to a study area using a shapefile
- Produce standardized, analysis-ready raster datasets for later units

This unit focuses on **data preparation**, not analysis.  
All later units (trend tests, SPI, spatial risk assessment) depend on the outputs created here.

---

## Conceptual workflow

The processing pipeline implemented in this unit is:

**Acquire → Normalize → Subset → Store**

1. **Acquire**  
   Bulk download the climate raster products from DWD.

2. **Preprocess data**  
   - Extract archives  
   - Convert to a common file format (GeoTIFF)  
   - Ensure a consistent CRS

3. **Subset**  
   Clip rasters to the spatial extent of the study area.

4. **Store**  
   Save standardized rasters in a reproducible folder structure.

---

## Input data

- Raw raster data from DWD (e.g. temperature, precipitation)
- A polygon dataset defining the study area (e.g. municipality boundary)

These inputs are stored in:
- 00_data\kerpen_shapefile
- 00_data\sample
