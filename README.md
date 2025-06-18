# Imputation Project 

## Project Organization 
- `raw_beiwe_data/`: Original, immutable raw data (read-only) collected from smartphone sensors
    - contains folders, each of which corresponds to a Beiwe id (unique identifier for each subject)
    - each subject folder contains a subfolder for a specific data stream. Some examples include:
        - `accelerometer/`: accelerometer data, where rows correspond to time stamps and columns correspond to x (latitude), y (longitude), z (elevation) coordinates in the Earth-Centered, Earth-Fixed (ECEF) Cartesian coordinate system.   
        - `gps\`: gps data, same structure as accelerometer data.
- `data/`: Cleaned data ready for analysis
- `docs/`: Documentation
  - `notes.md`: Notes on the project: To-Do, Discussions, etc.
- `src/R/`: Numbered analysis scripts showing workflow
  - `00_clean_data.R`: Data cleaning and preprocessing
  - `01_analysis.R`: Model fitting and analysis
  - `02_make_figures.R`: Figure generation
  - `03_report.Rmd`: Final report generation
- `sandbox/`: Exploratory analysis scripts
  - `01_frechet_rf.qmd:` Reproducing results from capitaine2024frechet
- `figs/`: Generated figures
- `refs/`: Reference materials
