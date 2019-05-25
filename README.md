# Tranformations for taking original data and transforming to Darwin Core
Cookbook of scripts to transform data for use in OBIS/GBIF and programs such as Pole to Pole

## Contacts
* Abby Benson (albenson@usgs.gov)
* Tylar Murray (tylarmurray@mail.usf.edu)
* Ben Best (bbest@ecoquants.com)

## Purpose
When transforming data from the data provider's original data format and aligning it with Darwin Core there are routine procedures that need to take place. 
The hope with this repository is that we can store some of those routine transformations and help reduce the burden on data providers in transforming their data.

Code reuse is complicated when it comes to data transforming (AKA munging) because datasets are often unique.
The goal of this repository is to collect together some examples of marine science data being transformed between various formats.

Examples should be relevant to OBIS, ERDDAP, DataOne data preparation (TODO: also [IOOS portal](https://mbon.ioos.us)?).

### Organizational Rules
* Examples should be in the form of `.md`, `.Rmd`, `.pynb`, or similar format.
* Examples should be organized by initial file format; this way someone with format `____` can easily find examples working with that format.
* Generally, examples should describe how to transform between only two formats. So a transformation from `.csv` and to DarwinCore and then DarwinCore to ERDDAP, that would actually be two separate examples.

## Examples
Here are a few examples from OBIS-USA for taking data from the original format to Darwin Core. 
Darwin Core term definitions can be found at:

occurrence- https://tools.gbif.org/dwca-validator/extension.do?id=dwc:Occurrence#Occurrence

event- https://tools.gbif.org/dwca-validator/extension.do?id=dwc:event

measurement or fact - https://tools.gbif.org/dwca-validator/extension.do?id=dwc:measurementorfact

OBIS-USA examples are stored in ScienceBase and include the data in its original format, the R script used for transforming
the data to Darwin Core, and the final files produced for the R script and harvested by OBIS and GBIF via the OBIS-USA IPT (https://www1.usgs.gov/obis-usa/ipt/).

Example 1 - NOAA Coral Percent Cover - original to Darwin Core Event Core with Extended Measurement or Fact
https://www.sciencebase.gov/catalog/item/55f33030e4b0ba2c1a007776

Example 2 - NOAA Florida Keys Reef Visual Census - original to Darwin Core Event Core with Extended Measurement or Fact
https://www.sciencebase.gov/catalog/item/57fe99a9e4b0824b2d14e2f2

Example 3 - USGS Great Lakes Science Center Trawl - original to Darwin Core Event Core with Extended Measurement or Fact
https://www.sciencebase.gov/catalog/item/5914eb0ae4b01a342e68ecdb

### More examples to add:
* FL Keys zooplankton -> OBIS : custom `.xlsx` -> DarwinCore Archive -> OBIS
* MODIS sat products -> ERDDAP : NetCDF `.nc` files -> ERDDAP
* NMSAS Occurence data : custom `.xlsx` -> DarwinCore Archive -> OBIS
* NMSAS water quality data : custom `.xlsx` -> IOOS?
* NMSAS benthic cover data : custom `.xlsx` -> ?
* [Data Wrangling in the R Tidyverse - Google Slides](https://docs.google.com/presentation/d/1fz00oSCm_cnJwgS1EoRvl1Mgd_j0i6lApILBAUO07jc/edit#slide=id.g32fcfaded4_0_105)
    * [Translate Dataset from DataOne to OBIS columns: SBC MBON](https://marinebon.github.io/sbc-datasets/)
    * [Introduction to Open Data Science](http://ohi-science.org/data-science-training/dplyr.html#group_by-operates-on-groups)
    * [Manipulating, analyzing and exporting data with tidyverse](https://datacarpentry.org/R-ecology-lesson/03-dplyr.html#reshaping_with_gather_and_spread)


# Additional Links
### Tools for working with data in OBIS/ERDDAP/DataOne/IOOS
* infographics with RVC / CREMP / IEA datasets
    * Monterey Bay Infographics: MB NMS
    * marinebon/info-fk: Infographics for Florida Keys: FK NMS
