# Overlap
## Overview
1) Data
2) R files
3) Dependencies

I recommend starting with overlap.pdf and then overlap.Rmd.

## Data
1) GIS files - (in folders CT*) sourced from the census bureau
2) zip_matrix.csv - weighting matrix for interpolating senate district data from zipcode level data.
3) Personal_wellbeing.csv - interpolatation the data used for the "personal wellbeing index" in the Indicator projects to the senate district level.
4) CWS data - NOT IN THIS REPO

## R files
1) overlap.Rmd - functions for producing zip_matrix.csv & personal_wellbeing.cs
2) overlap.pdf - an overview of the process and some data visualizations

## Dependencies
To produce a weighting matrix and maps:
1) sf - a streamlined geography package
2) tidyverse 
3) ggplot2 (development) see overlap.Rmd for more information

To interpolate CWS data
1) haven
2) tidyverse (dplyr)
