# Work Space

This folder contains the sensor-specific scripts used to perform the complete data cleaning, missing-value treatment, and imputation workflow for each environmental sensor analyzed in the capstone project.

Each script corresponds to a specific sensor and applies the reusable functions defined in `cleaning_stephanie.py`.

## Contents

The folder contains the scripts corresponding to the different environmental sensors analyzed in the project.

Each script follows the general workflow:

1. Load the raw sensor data from the `Data/` directory.
2. Perform initial data inspection and exploratory analysis.
3. Identify missing observations and potential anomalies.
4. Apply the selected cleaning procedures.
5. Compare the Z-score and percentile-based criteria where applicable.
6. Treat remaining missing observations.
7. Perform the imputation procedure.
8. Evaluate the resulting data.
9. Generate plots and summary results.

## Relationship with `cleaning_stephanie.py`

The functions used throughout these scripts are centralized in the `cleaning_stephanie.py` module located in the root directory of the repository.

This structure avoids duplicating the same functions across individual sensor scripts and ensures that the cleaning and imputation procedures are applied consistently across sensors.

## Sensor-Specific Scripts

Each script is self-contained with respect to the analysis of its corresponding sensor and documents the steps required to transform the raw observations into the cleaned and imputed dataset.

The scripts also contain the sensor-specific parameters, processing decisions, visualizations, and model configurations required for each analysis.

## Reproducibility

To reproduce the analysis for a specific sensor:

1. Ensure that the corresponding raw dataset is available in the `Data/` directory.
2. Open the corresponding sensor script.
3. Ensure that `cleaning_stephanie.py` is accessible from the project root.
4. Run the script from the repository environment.
5. Review the generated outputs and compare them with the summaries provided in the `Review/` directory.

The scripts are provided to document the complete analytical workflow used in the capstone project and to facilitate reproducibility of the results.
