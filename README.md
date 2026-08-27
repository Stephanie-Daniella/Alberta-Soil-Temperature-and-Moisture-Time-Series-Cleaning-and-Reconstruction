# Environmental Sensor Data Cleaning and Imputation

This repository contains the code, raw datasets, and supporting analyses developed for the cleaning and imputation of long-term environmental sensor data used in the capstone project.

The project focuses on identifying anomalous observations and imputing missing values in environmental time series while preserving their temporal structure.

## Repository Structure

```text
.
├── cleaning_stephanie.py
├── Work Space/
├── Review/
├── Data/
└── README.md
```

### `cleaning_stephanie.py`

This file contains the reusable functions developed for the project and used throughout the sensor-specific analysis scripts.

The module includes functions for:

* Data preprocessing and cleaning
* Anomaly detection and removal
* Z-score and percentile-based cleaning
* Missing-value identification
* Missing-value imputation

The functions were designed to provide a consistent workflow across the different environmental sensors analyzed in the project.

### `Work Space/`

This folder contains the scripts used to process each environmental sensor individually.

Each script presents the complete workflow for its corresponding sensor, including:

1. Data loading and preprocessing
2. Application of the cleaning procedures
3. Identification and treatment of missing observations
4. Imputation
5. Model fitting and evaluation, where applicable
6. Generation of results and visualizations

The scripts use the reusable functions defined in `cleaning_stephanie.py`.

### `Review/`

This folder contains the quantitative review of the datasets before and after the cleaning process.

The analyses include:

* Descriptive statistics of the raw and cleaned datasets
* Minimum, mean, and maximum values
* Number of missing observations
* Original number of observations
* Number of observations removed during cleaning
* Summary of the resulting datasets after cleaning

This folder provides a consolidated view of the effects of the cleaning procedures across the different sensors and study locations.

### `Data/`

This folder contains the raw environmental sensor datasets used in the project.

The data in this folder correspond to the original observations before the cleaning and imputation procedures were applied.

The raw datasets are preserved separately from the processed data to maintain a reproducible workflow and allow the cleaning and imputation procedures to be independently reviewed.

## Workflow

The general workflow followed in the project is:

```text
Raw Sensor Data
       │
       ▼
Predictor Variables Filling
       │
       ▼
Cleaning and Anomaly Detection of Temperature/Moisture
       │
       ├── Z-score Criterion
       │
       └── Percentile Criterion
       │
       ▼
Missing-Value Treatment
       │
       ▼
Imputation
       │
       ▼
Interesting Cases
```

The reusable functions are implemented in `cleaning_stephanie.py` and are called by the individual sensor scripts located in `Work Space/`.

## Reproducibility

To reproduce the analysis:

1. Review the raw datasets in `Data/`.
2. Select the corresponding sensor script from `Work Space/`.
3. Run the script using the functions provided in `cleaning_stephanie.py`.
4. Review the resulting statistics and comparisons in `Review/`.

The raw datasets are retained separately from the analysis scripts and processed results so that the original observations remain available for comparison and verification.

## Project Scope

This repository was developed as part of the capstone project for the Master of Science (MSc) in Mathematical and Statistical Sciences, with a specialization in Modeling, Data and Predictions (MDP) at the University of Alberta.

The project investigates statistical approaches for cleaning and imputing long-term environmental sensor time series. The primary objective was to identify and treat anomalous and missing observations while minimizing unnecessary alterations to the underlying temporal structure of the data.

This repository contains the code, raw datasets, and supporting analyses associated with the capstone project and contributes to the requirements for completion of the MSc degree.

This repository was developed as part of a capstone project investigating statistical approaches for cleaning and imputing long-term environmental sensor time series.

The primary objective was to identify and treat anomalous and missing observations while minimizing unnecessary alterations to the underlying temporal structure of the data.
