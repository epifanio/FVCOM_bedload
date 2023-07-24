# FVCOM_bedload

[![DOI](https://zenodo.org/badge/670196291.svg)](https://zenodo.org/badge/latestdoi/670196291)

Compute bedload transport from FVCOM 

Demonstration using the NetCDF4-Python library to compute bedload transport and bottom velocity (1 meter above bottom) from a triangular grid ocean model (FVCOM) via OPeNDAP.  The results are stored in a new NetCDF4 file. 

NECOFS (Northeastern Coastal Ocean Forecast System) is run by groups at the University of Massachusetts Dartmouth and the Woods Hole Oceanographic Institution, led by Drs. C. Chen, R. C. Beardsley, G. Cowles and B. Rothschild. Funding is provided to run the model by the NOAA-led Integrated Ocean Observing System and the State of Massachusetts.

NECOFS is a coupled numerical model that uses nested weather models, a coastal ocean circulation model, and a wave model. The ocean model is a volume-mesh model with horizontal resolution that is finer in complicated regions. It is layered (not depth-averaged) and includes the effects of tides, winds, and varying water densities caused by temperature and salinity changes.

## Model description 

    http://fvcom.smast.umassd.edu/research_projects/NECOFS/model_system.html
    
    
## Online data resources
* THREDDS server with other forecast and archive products: 

    http://www.smast.umassd.edu:8080/thredds/catalog.html


**Note:**
The notebook here calculates the **instantaneous bedload transport**. 
The **net transport** is given by averaging the results over a tidal cycle (average over an exact number of tidal cycles to don't get some fraction of a remaining tidal cycle affecting the mean)


**Author:** Rich Signell (USGS), Massimo Di Stefano (CCOM)
