# Data

The main data files are fish.csv and location.csv from bottom-trawl surveys in the Gulf of Alaska and west coast of Canada and U.S. from 1996 to 2015. The two datasets are quality controlled in Li et al. (2019) and the size classes of fish with fewer samples (e.g. the smallest and largest size classes) were further managed in the Get_Data function prior to analyses. 

The LW_DFO.csv includes data from the bottom-trawl survey conducted by Fisheries and Oceans Canada (DFO) off the west coast of Canada and only used for length-weight relationships in this region. 

▪	fish.csv contains all time series on fish related information including: CPUE, species, length (mm), frequency, and size class (BIN, at 100 mm interval). Additionally, it contains haul information including: survey, subregion, year, stratum, haul code (HAULJOIN), depth (m), longitude (LON, °), latitude (LAT, °N), and bottom temperature (TEMP, °C). Only non-zero catches were included for abundant species in each subregion (See species list in Li et al. 2019). Note that the unit for CPUE is number/km2 for each species (as a whole) in the Gulf of Alaska and U.S. west coast surveys while CPUE is kg/m2 for the Canadian west coast survey. 

▪	location.csv contains all valid hauls regardless if there are any fish of interest caught in a haul.  Therefore, more hauls are included than found in fish.csv. In addition to the haul-related columns in the fish.csv, location.csv also contains the area for each stratum.

▪	LW_DFO.csv is used to estimate length-weight relationships to split CPUE of the whole species into size classes for the DFO survey along the Canadian west coast. It contains subregion, year, species, length (mm), and weight (g). Fish length was measured in all hauls in fish.csv, but individual weight was only measured in some hauls in LW_DFO.csv; therefore, a species-specific length-weight relationship was estimated and applied to all DFO survey data in fish.csv.


References

Li L, Hollowed AB, Cokelet ED, Barbeaux SJ, Bond NA, Keller AA, King JR, McClure MM, Palsson WA, Stabeno PJ, and others (2019) Subregional differences in groundfish distributional responses to anomalous ocean bottom temperatures in the northeast Pacific. Global Change Biology 25:2560-2575

