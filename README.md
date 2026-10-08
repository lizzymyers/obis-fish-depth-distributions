# obis-fish-depth-distributions
Analysis and visualisation of fish occurrence records from the Ocean Biodiversity Information System (OBIS), with a focus on species, genus and family distributions across depth.

## Overview

This repository contains an R-based workflow for retrieving, cleaning and visualising OBIS occurrence records for selected fish taxa.

The workflow is designed to be reusable: a focal species, genus and family are specified at the beginning of the analysis, and the subsequent taxonomic summaries and depth-distribution analyses are generated automatically.

## Analyses

The workflow currently includes:

- Retrieval of occurrence records from OBIS
- Taxonomic filtering and validation
- Summary of species richness within the focal family
- Comparison of genera within families
- Species occurrence distributions across depth
- Visualisation of depth distributions
- Automated generation of taxon-specific HTML reports

## Repository structure

```text
obis-fish-depth-distributions/
│
├── OBIS_depth_distribution_analysis.ipynb
├── reports/
├── README.md
└── .gitignore
```

### `OBIS_depth_distribution_analysis.ipynb`

The main analysis notebook. The notebook uses an R kernel and is intended to be reused for different taxa by changing the focal species, genus and family at the beginning of the analysis.

### `reports/`

Rendered HTML reports generated for individual taxa.

## Software

The analysis is conducted in **R** using a **Jupyter Notebook**.

Key R packages include:

- `robis`
- `dplyr`
- `ggplot2`
- `IRdisplay`

Additional package requirements are documented within the notebook.

## Data source

Occurrence data are obtained from the **Ocean Biodiversity Information System (OBIS)**.

OBIS: https://obis.org/

Users of these analyses should consult the OBIS data policy and appropriately acknowledge the individual datasets contributing occurrence records.

## Reproducibility

To run an analysis:

1. Open `OBIS_depth_distribution_analysis.ipynb` using an R Jupyter kernel.
2. Specify the focal species, genus and family in the taxon-selection section.
3. Run the notebook from top to bottom.
4. Export the completed analysis as an HTML report.

Output filenames are generated automatically from the focal family, genus and species.

## Author

Lizzy Myers
