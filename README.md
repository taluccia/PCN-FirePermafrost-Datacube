# Permafrost Carbon Network Synthesis Estimated FireALT Dataset


## Overview

This repo includes scripts for development of a synthesized dataset of estimate active layer thickness of burned/unburned sites across the high northern latitudes. 

## Scripts

1. `DataCleanToPointCombine.Rmd` --- This script takes each data contribution and checks abnormalities and formatting issues. It fixes any issues. Data is then combines into a single data frame and converted in to a spatial data set and saved as a shapefile. 
2. `ERA5GeeScript.Rmd` --- GEE Script for pulling ERA5 data using JavaScript Code editor.
3. `ERA5CleanOrganizeData.Rmd` --- Takes the EE ERA5 Land Temperature data and organize it into a single csv.
4. `EstimateALT.Rmd` --- Takes the output from 3 and predict ALT measurements.
5. `PlotLevelAggregate.Rmd` --- Takes the output from 3 and predict ALT measurements.
6. `SpatialAdds.Rmd` ---This scripts takes the output from step 1 and adds spatial attributes including ecozones and permafrost extent.
7. `PairsAggregate.Rmd` --- Takes the output from 6 and aggregates the data by burned-unburned pairs.

--- No Longer needed
8. `FinalizeAttributes.Rmd` --- Takes the output from 5 and finalizes attributes.


