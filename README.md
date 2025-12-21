# Satellite Night Lights and Economic Growth in Laos

This repository contains the code and resources used in the analysis of how satellite night light intensity can be used as a proxy for economic activity and growth across regions in Laos.

The purpose of this repository is to support transparency and reproducibility for the study.

---

## Structure

- `code/` — Jupyter notebooks and scripts used for preprocessing, aggregating, and visualizing satellite night lights.
- `data/` — Information about datasets used (raw files not included due to size).
- `figures/` — Visualizations such as heat maps and time-series plots.
- `docs` — Project report and slides.

---

## Data Sources

Nighttime light data can be downloaded from the VIIRS database hosted by the Payne Institute / NOAA:

https://eogdata.mines.edu/nighttime_light/annual/v21/

To reproduce the analysis:

- download annual VIIRS night-light files (e.g., 2014–2023)
- extract the `.tif` files for each year
- place them in a folder (e.g., `NTL_data`)
- update the file paths in the notebook accordingly

Administrative boundary shapefiles for Laos can be downloaded from:

- https://gadm.org  
or  
- Open Development Laos

---

## Code

The main notebook performs:

- aggregation of luminosity at province/district level
- winsorization to reduce outlier effect
- loops over time to compute growth
- visualization through heat maps and line charts

Example file:
- `nightlights_laos_analysis.ipynb`

---

## Running Locally

Clone the repository:

```bash
git clone https://github.com/zeyasoukhabandith/laos-economic-growth-satellite-data.git
