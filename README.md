# Introduction 

This is the repository for the code related to the paper

Gaetan, C., Opitz, T. and Toulemonde, G. (2024+), Statistical modeling of extreme precipitation, In M. de Carvalho, R. Huser, P. Naveau, & B. J. Reich (Eds)
Handbook on Statistics of Extremes. Chapman & Hall / CRC.  Boca Raton, FL.

# Data description


- yearMax: This file contains aggregated rainfall data over different durations and for different stations.
- meta.csv: This file contains additional information of the different stations 
          such as longitude, latitude, altitude, temporal resolution (m=minutely, h=hourly, d=daily), group. The same group is assigned to stations which have a distance of less than 250 meters and can be treated as one station.

  These data were used in the study “Flexible and Consistent Quantile Estimation for Intensity-Duration-Frequency Curves” (Fauer et al., 2021) 
See https://zenodo.org/records/5012621 for more details and for the original source. 


- daily_rainfall_germany.Rdata: Daily precipitation data recorded in 191 meteorological stations ((period 1st January 1923 - 31st December 2023). 
		              Source: German Weather Service (Deutscher Wetterdienst, DWD) (ftp://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/daily/more_precip/historical/)
                              The dataset is retrieved using the rdwd package (https://bookdown.org/brry/rdwd/). 
                              See the script the Rmarkdown script Get-daily-data-Germany.Rmd


- single-daily.Rdata: Daily precipitation data recorded at  Jena (period 1st January 1827 - 8th August 2019). 
                    Source: German Weather Service (Deutscher Wetterdienst, DWD). See the Rmarkdown script Get-daily-data-single-station.Rmd


# Code


	
- Get-daily-data-Germany.Rmd : Script to get Jena data

- Get-daily-data-single-station.Rmd: Script to get all station data

- Estimation-daily-data.Rmd : Script for applying different estimation methods to the Jena data
	
- IDF-example.Rmd : Example of IDF curve estimation

- Regression-with-GAM.Rmd :

# REFERENCES

Gaetan, C., Opitz, T. and Toluemonde, G. (2024), Statistical modeling of extreme precipitation, In M. de Carvalho, R. Huser, P. Naveau, & B. J. Reich (Eds)
Handbook on Statistics of Extremes. Chapman & Hall / CRC.  Boca Raton, FL.
