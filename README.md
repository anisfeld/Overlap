# Overlap
## Overview
1) Data
2) R files
3) Dependencies

I recommend starting with [overlap.pdf](https://github.com/anisfeld/Overlap/blob/master/overlap.pdf) and then exploring the code in [overlap.Rmd](https://github.com/anisfeld/Overlap/blob/master/overlap.Rmd)

DataHaven, a Connecticut-based non-profit data consultancy, conducts the Community Wellbeing Survey every three years to provide more holistic metrics to inform decisionmaking. The purpose of Overlap is to interpolate survey data collected at the zip-code level to state senate districts so that our clients can use Community Wellbeing Survey data to drive approach to advocating for reforms.

The document has two sections. First, we create a zip-code to senate district weight matrix and, second, we apply it to CWS data to interpolate senate districts data from the zipcode level. The two parts are nearly self-contained as the main output from the first part is saved in a csv that is accessible in the folder. Unless you are particularly intersted in playing with the geographic data / maps, I recommend reading through part 1 and then doing part 2 interactively.


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
