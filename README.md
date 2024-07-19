# PCN-FirePermafrost-Datacube


## Overview

This repo includes scripts for development of a synthesized datacube of burned/unburned permafrost thaw measurements across the high northern latitude permafrost zone. 

## Scripts

1. `DataCleanToPointCombine.Rmd` --- This script takes each data contribution and checks abnormalities and formatting issues. It fixes any issues. Data is then combines into a single data frame and converted in to a spatial data set and saved as a shapefile. 
2. `SpatialAddsDatacube.Rmd` ---This scripts takes the output from step 1 and adds spatial attributes including ecozones and permafrost extent.
3. `ERA5GeeScript.Rmd` --- GEE Script for pulling ERA5 data using JavaScript Code editor.
4. `ERA5CleanOrganizeData.Rmd` --- Takes the EE ERA5 Land Temperature data and organize it into a single csv.
5. `PredictAltMeasurements.Rmd` --- Takes the output from 4 and predict ALT measurements.
6. `FinalizeDatacubeAttributes.Rmd` --- Takes the output from 5 and finalizes attributes.
7. `AggregatePairedBurnUnburn.Rmd` --- Takes the output from 6 and aggregates the data by burned-unburned pairs.
