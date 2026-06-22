# Understanding, characterizing, and modeling compound hazards for urban resilience



This repository contains the data processing, exploratory analysis, and visualization workflows used to analyze compound hazards using the EM-DAT (Emergency Events Database) and related literature datasets.

The project focuses on:

- Cleaning and restructuring EM-DAT disaster records
- Extracting and classifying associated hazard types
- Exploring temporal trends in compound hazards
- Visualizing hazard interactions and publication trends



## EM-DAT analysis  (`01_emdat.ipynb`)
### Data sources

EM-DAT contains data on the occurrence and impacts of over 27,000 mass disasters worldwide from 1900 to the present day.

Official website:

https://www.emdat.be/

### EM-DAT processing

In EM-DAT, the field records "*associated types*", defined as subsequent or co-occurring hazards that may have contributed to the overall disaster impact. We use this field as a proxy for compound hazards.

This notebook performs:

- Loading and filtering EM-DAT records
- Separating natural and technological disasters
- Parsing associated hazard types
- Expanding multi-hazard relationships into structured columns
- Using the Louvain algorithm to identify hazard clusters
- Creating yearly summaries and descriptive statistics
- Preparing outputs for visualization and network analysis

Data availability:

The raw and processed datasets used in this study are available in the `data` directory of the associated repository.

## Trend analysis (`02_trend_analysis.ipynb`)
This notebook focuses on publication and methodological trends of modeling compound hazards. Methods include physics-based methods, data-driven methods, and hybrid methods.

Main analyses include:

- Annual publication counts
- Methodological evolution over time
- Distribution of spatial scales
- Compound hazard type frequencies
- Visualization of research trends

Data availability:

The processed datasets supporting the findings of this systematic review are available from the authors upon reasonable request.