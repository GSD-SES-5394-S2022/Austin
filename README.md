# Austin Travel Demand Model

This repository consists of code and data that is being used to build a travel demand model for the Austin-Round Rock, TX metropolitan statistical area. This is a term project for the course SES 5394 Travel Behavior and Forecasting, taught at the Harvard Graduate School of Design in Spring 2022. 

The goal of this project is compare two alternatives and assess differences in travel patterns. One is a representation of existing conditions, with some simplifications made for tractability. The other is an alternative where streets in a portion of Downtown Austin are closed to private vehicles, though walking, bicycling, and transit may still access them. We hope to observe any changes in overall mobility, VMT, and mode share, as the area with road closures is a major employment hub but is served well by public transit.

Data and scripts for this project are contained in the following subfolders:

* *assignment rmd docs* - R Markdown files used to generate content used in reports (folder a*x* corresponds to Assignment *x*), and an archive of older code used for initial experimentation that may be useful to have as a reference in the future
* *images* - folder for saving visualizations, broken down by assignment
* *existing* - population and employment data for the census tracts in the MSA, as well as transportation network data (GTFS for Capital Metro and the MSA road network) 
* *alternative* - population data unchanged from *existing*, as our proposal does not affect population, employment, or land use, only the transportation network. The alternative road network is modified so that private vehicles may not enter Downtown Austin (bounded by I-35, Cesar Chavez St, Lamar Blvd, and Martin Luther King Jr. Blvd)
* *zones* - spatial data for each of the census tract TAZs
* *commutes* - additional data on current commuting patterns, so far only used in Assignment 2 visualization

The following R Markdown files are used to perform this analysis (list to be updated over the course of the semester):

* *a2.Rmd* - generates tract-level TAZs and associated population/employment data for the MSA (assignment rmd docs/a2)
* *a4_networks.Rmd* - downloads public transit and road network data for Austin. (assignment rmd docs/a4)
* *a4_skims.Rmd* - calculates travel time by mode between TAZ centroids with maps comparing existing conditions to the alternative (assignment rmd docs/a4)
* *a5_access* - calculates job accessibility by mode for each TAZ in existing conditions and alternative scenario; saves them in *csvs* sub-folder (assignment rmd docs/a5)
* *a5_graphics* - mapping and visualization for assignment 5
* *a6_model* - creates model to estimate change in number of zero-car households in the alternative, as well as visualizations 