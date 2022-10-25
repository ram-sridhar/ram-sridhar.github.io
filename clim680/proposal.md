# The relative role of high-frequency and low-frequency wind forcing on El Niño development
 
### Sridhar Mantripragada
#### CLIM 680 - Fall 2022

## Introduction

My CLIM 680 project investigates the relative role of high-frequency and low-frequency wind forcing on El Niño development. The precursor and trigger for the El Niño growth are anomalous positive ocean heat content and wind forcing over the western Pacific, respectively. The wind forcing has broad frequency range spread over low-frequencies (> 90-day) and high-frequencies (< 90-day). 

The mechanims behind the ENSO growth has been widely explored and written about in the scientific literature. However, there is a debate on whether it is the low-frequency (> 90-day) not related to ENSO or high-frequency (< 90-day) wind forcing that triggers the Bjerkness feedback and thus El Niño growth. 

I wanted to revist this topic and investigate the relative role of different frequency band wind forcing on El Nino growth using the intermediate complex coupled model -  Zebiak and Cane (ZC). 



## Data

The datasets used in my project are:

__NOAA/OISST__
The [NOAA/OISST](https://www.ncei.noaa.gov/products/optimum-interpolation-sst) dataset is daily, 
global sea surface temperature data from Jan, 1980 to Dec, 2016. It has horizontal resoluiton of 0.25deg longitude by 0.25deg latitude.
 
__INCOIS/TropFlux/wind stress__
The [TropFlux wind stress](https://kpegion.github.io/COLA-DATASETS-CATALOG/gpcp_precip.mon.mean.nc) is daily tropical 
wind stress from Jan 1980 to Dec 2016. It is on a 1deg longitude by 1deg latitude grid.

__INCOIS/TropFlux/SST__
The [TropFlux SST](https://kpegion.github.io/COLA-DATASETS-CATALOG/ghcn_cams) is daily tropical 
SST from Jan 1980 to Dec 2016. It is on a 1deg longitude by 1deg latitude grid.

## Model

Zebiak-Cane (ZC; Zebiak and Cane 1987)

The ZC model is used to perform control and sensitivity experiments which will help to disentagle the ambiguity surrounding the relative importance of low-frequency and high-frequency wind forcing on El Nino development given the western Pacific is primed with positive ocean heat content anomlaies.


## Proposed Analysis
I plan to use the data sets above to conduct the following analysis:
* Calculate climatology and anomalies of observed SST and wind stress
* Perform forced and unforced ZC model runs.
* Calculate the Niño3 and Niño3.4 index from the observed and simulated SST data
* Calculate the power spectrum of wind stress and SST for equatorial Pacific.
* Calculate the means of ensemble members simulated fields 
* Calculate and compare composites of control and sensitivity experiements variables
* Calculate the ensemble mean difference between the control and sensitivity experiements variables with significane
* Calculate the regression of Nino3.4 with wind stress to linearly remove the contemporaneous impact of ENSO on wind stress

### Functions
I will create a set of functions in `clim_utils.py` for doing common tasks used throughout my analysis, including:
* Labelling plots
* calculating climatology and anomalies
* etc.

### Conda Environment

The environment.yml file is provided to define the environment needed to run all codes.
