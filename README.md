# MTAC Fire Simulation

This project includes Jupyter notebooks and data for simulating aerial fire response in Iligan City, Philippines.

## Notebooks

- `MTAC-Extracting Iligan City Data.ipynb` – downloads and processes barangay and road data
- `MTAC-FORECASTING POPULATION.ipynb` – forecasts 2030 population using regression models
- `MTAC-MainSimulation.ipynb` – runs the simulation model using the input data

## Data Files

All required input files (such as shapefiles, CSVs, and GraphML files) are stored in the following shared Google Drive folder:

https://drive.google.com/drive/folders/1ztcHIqi_StGcTbFYGvohaAez1s8xYzNy

Download the files and place them in a `data/` folder located in the same directory as the notebooks.

## LaTeX Report

The `latex/` folder contains the final written report in LaTeX format, including:
- `main.tex`: Main document
- `bibliography.bib`: References
- `figures/`: Visuals used in the report

To compile:
1. Install `pdflatex`, `bibtex`
2. Run:
   pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex

## Important Notes

Some paths in `MTAC-MainSimulation.ipynb` refer to files located on the author’s local machine. To run this notebook:

1. Download all required files from the Google Drive folder linked above.
2. Place the files inside a folder named `data/`.
3. Modify the file paths inside the notebook if necessary.

## Requirements

To run the notebooks, install the following Python packages:

- pandas
- geopandas
- osmnx
- networkx
- matplotlib
- scikit-learn
- gdown
