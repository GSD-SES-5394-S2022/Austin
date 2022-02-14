# Austin Travel Demand Model

This repository consists of code and data that is being used to build a travel demand model for the Austin-Round Rock, TX metropolitan statistical area. This is a term project for the course SES 5394 Travel Behavior and Forecasting, taught at the Harvard Graduate School of Design. 

The goal of this project is compare two alternatives and assess differences in travel patterns. One is a representation of existing conditions, with some simplifications made for tractability. The other is an alternative where streets in a portion of Downtown Austin are closed to private vehicles, though walking, bicycling, and transit may still access them. We hope to observe any changes in overall mobility, VMT, and mode share, as the area with road closures is a major employment hub but is served well by public transit.

Data for this project is contained in the following subfolders:
* *existing* - population and employment data for the census tracts in the MSA that we are using as TAZs for our analysis
* *alternative* - unchanged from *existing*, as our proposal does not affect population, employment, or land use, only the transportation network
* *zones* - spatial data for each of the census tract TAZs
* *commutes* - additional data on current commuting patterns, so far used in Assignment 2 visualization

The following R Markdown files are used to perform this analysis (list to be updated over the course of the semester):

* *assignment2.Rmd* - generates tract-level TAZs and associated population/employment data
* *assignment3.Rmd* - 
