# NYSERDA-Branscomb-Solar-NDVI
NDVI Paired t-test on NYSERDA Branscomb Solar

---

## Description
Visualizes paired t-test on the Normalized Difference Vegetation Index (NDVI) of Pre-Construction (2020) and Post-Construction (2022) of NYSERDA Branscomb Solar Farm commissioned and built April 2021. A control variable of 8 nearby randomly-sampled grass fields are included.

---

#### Subdirectory Info:
1. raw-data
    + NYSERDA Branscomb Solar shapefile
    + Sentinel-2 NDVI raster tif during 4 month periods (cloud masked in Google Earth Engine)
2. processed-data
    + Branscomb Solar edge buffers (10-40 meters away from solar collections) shapefiles processed in QGIS
    + Sentinel-2 NDVI changes during 4 month periods (January-April, May-August, September-December) from 2020 to 2022 tif files
3. results
    + Pre- & Post-Construction NDVI pixel frequency .csv (exported from QGIS)
4. figures
    + Average Branscomb Solar edge NDVI from 2020 - 2023 graph
    + Paired t-test results for NDVI 4-month periods on Branscomb Solar edge and control variable
    + Images of pixel frequency histograms in NDVI raster (from QGIS)
        + *Note: To ensure normal distribution needed to perform paired t-test*
    +  Boxplot of paired t-test results of NDVI on Branscomb Solar edge and control variable
5. rmarkdowns
    + rmarkdown script code chunks to create paired t-test & boxplots for NDVI Branscomb Solar edge buffer and control variable
        + *Note: may need to import .csv dataset in `results` subdirectory to run script*
