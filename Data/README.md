# Data

This folder contains the raw environmental sensor datasets used in the capstone project.

The datasets contain long-term environmental measurements collected from multiple monitoring locations in Alberta. The data include the environmental variables used throughout the analysis, including temperature, humidity, radiation, wind speed, soil temperature, and soil moisture measurements.

## Raw Data

The datasets in this folder correspond to the original observations obtained from the environmental monitoring sources before any cleaning, anomaly detection, or imputation procedures were applied.

No observations were removed or imputed in these files. The raw datasets are preserved to provide a reference point for the entire analytical workflow and to support reproducibility.


## Directory Structure

```text
Data/
├── Brocket/
│   ├── * AGDM.*
│   ├── *_AGDM.*
│   ├── *_air_temp_precip.*
│   └── *_humidity_wind_radiation.*
│
├── Champion/
│   ├── * AGDM.*
│   ├── *_AGDM.*
│   ├── *_air_temp_precip.*
│   └── *_humidity_wind_radiation.*
│
├── Champion/
│   ├── * AGDM.*
│   ├── *_AGDM.*
│   ├── *_air_temp_precip.*
│   └── *_humidity_wind_radiation.*
│
├── Foremost/
│   ├── * AGDM.*
│   ├── *_AGDM.*
│   ├── *_air_temp_precip.*
│   └── *_humidity_wind_radiation.*
├── Manning/
│   ├── * AGDM.*
│   ├── *_AGDM.*
│   ├── *_air_temp_precip.*
│   └── *_humidity_wind_radiation.*
├── rich Lake/
│   ├── * AGDM.*
│   ├── *_AGDM.*
│   ├── *_air_temp_precip.*
│   └── *_humidity_wind_radiation.*
└── ...
```

Each location folder contains four raw datasets, grouped according to the type of environmental measurements they contain.

