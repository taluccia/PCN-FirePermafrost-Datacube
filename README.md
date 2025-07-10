# Permafrost Carbon Network Synthesis Estimated FireALT Dataset


This repository contains scripts central to the following data synthesis effort that includes a publish data set and accompanying data paper listed below. The scripts were used for the development of a synthesized data set of estimate active layer thickness of burned/unburned sites across the high northern latitudes. 

- Talucci, A., M. Loranty, J. Holloway, B. Rogers, H. Alexander, N. Baillargeon, J. Baltzer, L. Berner, A. Breen, L. Brodt, B. Buma, C. Delcourt, L. Diaz, C. Dieleman, T. Douglas, G. Frost, B. Gaglioti, R. Hewitt, T. Hollingsworth, M. T. Jorgenson, M. Lara, R. Loehman, M. Mack, K. Manies, C. Minions, S. Natali, J. O’Donnell, D. Olefeldt, A. Paulson, A. Rocha, L. Saperstein, T. Shestakova, S. Sistla, S. Oleg, A. Soromotin, M. Turetsky, S. Veraverbeke, and M. Walvoord. 2024. FireALT dataset: estimated active layer thickness for paired burned unburned sites measured from 2001-2023. Arctic Data Center.

- Talucci, A., M. M. Loranty, J. E. Holloway, B. M. Rogers, H. D. Alexander, N. Baillargeon, J. L. Baltzer, L. T. Berner, A. Breen, L. Brodt, B. Buma, J. Dean, C. J. F. Delcourt, L. R. Diaz, C. M. Dieleman, T. A. Douglas, G. V. Frost, B. V. Gaglioti, R. E. Hewitt, T. Hollingsworth, M. T. Jorgenson, M. J. Lara, R. A. Loehman, M. C. Mack, K. L. Manies, C. Minions, S. M. Natali, J. A. O’Donnell, D. Olefeldt, A. K. Paulson, A. V. Rocha, L. B. Saperstein, T. A. Shestakova, S. Sistla, O. Sizov, A. Soromotin, M. R. Turetsky, S. Veraverbeke, and M. A. Walvoord. 2024, December 3. Permafrost-wildfire interactions: Active layer thickness estimates for paired burned and unburned sites in northern high-latitudes. Copernicus GmbH.

[Link to data set](https://arcticdata.io/catalog/view/doi%3A10.18739%2FA2RN3092P)

[Link to paper](https://doi.org/10.5194/essd-17-2887-2025)


## Scripts

1. `DataCleanToPointCombine.Rmd` --- This script takes each data contribution and checks abnormalities and formatting issues. It fixes any issues. Data is then combines into a single data frame and converted in to a spatial data set and saved as a shapefile. 
2. `ERA5GeeScript.Rmd` --- GEE Script for pulling ERA5 data using JavaScript Code editor.
3. `ERA5CleanOrganizeData.Rmd` --- Takes the EE ERA5 Land Temperature data and organize it into a single csv.
4. `EstimateALT.Rmd` --- Takes the output from 3 and predict ALT measurements.
5. `PlotLevelAggregate.Rmd` --- Takes the output from 3 and predict ALT measurements.
6. `SpatialAdds.Rmd` ---This scripts takes the output from step 1 and adds spatial attributes including ecozones and permafrost extent.
7. `PairsAggregate.Rmd` --- Takes the output from 6 and aggregates the data by burned-unburned pairs.


