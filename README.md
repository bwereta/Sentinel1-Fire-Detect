# SENTINEL-1 Wildfire Classification

This project uses **Sentinel-1** polarimetric data to generate **fire perimeter** and **burn severity** maps using VH polarization backscatter.  
The input Sentinel-1 data should already have **Radiometric Terrain Correction (RTC)** applied, especially for areas with terrain shadows.

---

## Project Overview

This repository provides tools and workflows for:  
- **Fire perimeter mapping**  
- **Burn severity classification**  
- **Image preprocessing and segmentation**  

The workflow leverages Sentinel-1 VH polarization backscatter to produce accurate wildfire mapping outputs.

---

## File Descriptions

### Jupyter Notebooks
- **`crop_image.ipynb`**  
  Crop raster images using fire perimeter boundaries provided in **GeoJSON** or **shapefile** format.
  
- **`preprocessing_segmentation.ipynb`**  
  Preprocess images and perform **superpixel segmentation**. Intermediate outputs are saved for future steps.
  
- **`perimeter_generation.ipynb`**  
  Generate the **fire perimeter** map from preprocessed Sentinel-1 data.
  
- **`burn_severity_generation.ipynb`**  
  Generate the **burn severity** map, including preprocessing steps.

---

### Python Scripts
- **`process_utils.py`**  
  Utility functions for merging **GeoJSON** fire perimeters or **burn severity** images.
  
- **`data_prep.py`**  
  Prepares input data for analysis and processing.
  
- **`run_analysis.py`**  
  Runs the full **analysis pipeline** for fire perimeter and burn severity mapping.

---

## Environment Setup

To create the required conda environment, run:
```bash
conda env create -f environment.yml
conda activate sentinel1-wildfire
