SENTINEL-1_wildfire_classification

This product uses SENTINEL-1 polarimetric data to generate fire perimeter and burn severity maps from VH polarization backscatter.
SENTINEL-1 data for study areas containing terrain shadow and This data alread run radiometric_terrain_correction(RTC).

Data Info

File Descriptions

Jupyter Notebooks

crop_image.ipynb: Crop the raster image by a fire perimeter in GeoJSON or shapefile format.
preprocessing_segmentation.ipynb: Preprocess the images and perform superpixel segmentation. Outputs are saved for future use.
perimeter_generation.ipynb: Generate the fire perimeter map.
burn_severity_generation.ipynb: Generate the burn severity map (preprocessing happens here).

Python Scripts

process_utils.py: Utility functions for merging GeoJSON (perimeter) or images (severity).
data_prep.py: Prepare data for processing.
run_analysis.py: Run the main analysis pipeline.

Environment Setup

environment.yml: Conda environment configuration file.

Environment Setup

environment.yml: Conda environment configuration file.
