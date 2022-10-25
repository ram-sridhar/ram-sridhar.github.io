# The relative role of high-frequency and low-frequency wind forcing on El Ni$~{n}$o development
 
### Sridhar Mantripragada
#### CLIM 680 - Fall 2022

## Introduction

My CLIM 680 project investigates the relationship between the El Nino Southern Oscillation and temperature and precipitation.  
I choose this topic because there is no consensusit has been widely explored and written about in the scientific literature, 
but I wanted to see these relationships for myself.  
I also explored the relationship between temperature and precipitation with another climate index, the NAO, for comparison.

## Data

The datasets used in my project are:

__NOAA/OISST__
The [NOAA/OISST](https://kpegion.github.io/COLA-DATASETS-CATALOG/sst.mnmean.nc) dataset is monthly, 
global sea surface temperature data from Dec, 1981 to Apr, 2020. It has horizontal resoluiton of 1deg longitude by 1deg latitude.
 
__GPCP Precipitation__
The [GPCP precipitation](https://kpegion.github.io/COLA-DATASETS-CATALOG/gpcp_precip.mon.mean.nc) is monthly global 
precipitation from Jan 1979 to Apr 2020. It is on a 2.5 deg longitude by 2.5 deg latitude gride.

__GHCN_CAMS__
The [GHCN_CAMS](https://kpegion.github.io/COLA-DATASETS-CATALOG/ghcn_cams) is a global, land-only, monthly temperature 
datasets from Jan 1948 to Mar 2020.  It is on a 0.5 deg longitude by 0.5 deg latitude grid.

__NAO Index__
The [NAO Index](https://www.psl.noaa.gov/data/correlation/nao.data) is the monthly CPC index, provided by NOAA/ESRL/PSL. 
It is located on the COLA servers in `/shared/ccsm4/kpegion/obs2/CLIM_INDICES/nao.data`. 

## Proposed Analysis
I plan to use the data sets above to conduct the following analysis:
* Calculate annual mean, climatology and anomalies of SST, precipitation and temperature
* Calculate the Niño3.4 index from the SST data
* Calculate composites of climate variables based on ENSO phases
* Calculate the mean difference between composites of El Niño and La Niña phases with significance
* Calculate and compare composites with the NAO index
* Calculate the regression of Nino3.4 with Temperature and Precipitation

### Functions
I will create a set of functions in `clim_utils.py` for doing common tasks used throughout my analysis, including:
* Labelling plots
* calculating climatology and anomalies
* etc.

### Conda Environment

The environment.yml file is provided to define the environment needed to run all codes.
