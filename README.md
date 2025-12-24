# Satellite Night Lights and Economic Growth in Laos

This repository contains the code, data references, and visual outputs used to analyze economic growth patterns in Laos using satellite night-light intensity as a proxy for economic activity. The project leverages VIIRS nighttime light data to examine spatial and temporal variations in development at the provincial and district levels.

The analysis focuses on identifying regional growth disparities, urban–rural differences, and development corridors by tracking changes in luminosity over time. Satellite-based measures provide valuable insights in contexts where official economic statistics may be limited, incomplete, or infrequently reported.

The purpose of this repository is to support transparency and reproducibility by documenting the data sources, methodology, and code used in the study.

---

## Repository Structure

- `code/` — Jupyter notebooks and scripts used for data preprocessing, aggregation, and analysis.
- `data/` — Data references, metadata, and documentation (raw satellite files not included due to size).
- `figures/` — Maps, plots, and visualizations generated from the analysis.
- `docs/` — Written analysis, report, and presentation materials.

---

## Data Sources

Nighttime light data are obtained from the VIIRS dataset hosted by the Payne Institute / NOAA:

https://eogdata.mines.edu/nighttime_light/annual/v21/

To reproduce the analysis:
- Download annual VIIRS nighttime light files for the relevant years
- Extract the `.tif` files into a single directory
- Update file paths in the analysis notebook accordingly

Administrative boundary shapefiles for Laos are sourced from publicly available geographic databases such as GADM or Open Development Laos.

---

## Methodology

The analysis includes:
- Aggregation of night-light intensity at the provincial and district levels
- Winsorization to mitigate the influence of extreme outliers
- Temporal analysis to track changes in luminosity over time
- Visualization using maps, heat plots, and time-series charts

These methods allow for comparison of growth patterns across regions and over time.

---

## Running the Code

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/laos-economic-growth-satellite-data.git
