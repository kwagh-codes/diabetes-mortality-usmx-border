# data/

This folder is **not tracked by Git** and is empty in the repository.

All data files required to reproduce the analysis are archived on Zenodo:

> **[https://doi.org/10.5281/zenodo.XXXXXXX](https://doi.org/10.5281/zenodo.19246775)**

## How to populate this folder

1. Download the three ZIP files from the Zenodo record above: `raw.zip`, `external.zip`, `processed.zip`
2. Extract each ZIP into this folder so the structure looks like:

```
data/
├── raw/
│   ├── inegi_mexico/
│   │   ├── defunciones_base_datos_2018_dbf/
│   │   ├── defunciones_base_datos_2019_dbf/
│   │   ├── defunciones_base_datos_2020_dbf/
│   │   ├── defunciones_base_datos_2021_dbf/
│   │   ├── defunciones_base_datos_2022_dbf/
│   │   └── defunciones_base_datos_2023_dbf/
│   ├── conapo_mexico/
│   │   ├── Population projections by municipals by year 2018-23.csv
│   │   └── Population projections by municipals by age sex group May 27, 2025.csv
│   ├── cdc_wonder_usa/
│   │   ├── Multiple Cause of Death 2018-2023 county level 2018-23 cleaned.csv
│   │   └── Multiple Cause of Death 2018-2023 county level 2018-23 by age groups.csv
│   └── gbd/
│       └── GBD_diabetes_2021_USMX.rds
├── external/
│   └── shapefiles/
│       ├── 00mun.shp  (+ .dbf .prj .shx)
│       ├── 00ent.shp  (+ .dbf .prj .shx)
│       ├── tl_2024_us_county.shp  (+ companions)
│       └── tl_2024_us_state.shp   (+ companions)
└── processed/
    ├── map_data_counties_USMX.rds
    ├── map_data_states_USMX.rds
    └── GBD_diabetes_2021_map_data_states_USMX.rds
```

## Note on `processed/`

The `processed/` folder is generated automatically when you render
`qmd/1__County_Level_DM_Mortality_2018-2023.qmd`. Downloading it from
Zenodo is optional — only do so if you want to skip running File 1 and
go straight to File 2.
