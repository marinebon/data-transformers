# Tranformations for taking original data and transforming to Darwin Core
Cookbook of scripts to transform data for use in OBIS/GBIF and programs such as Pole to Pole

## Contacts
Abby Benson (albenson@usgs.gov)

## Purpose
When transforming data from the data provider's original data format and aligning it with Darwin Core there are
routine procedures that need to take place. The hope with this repository is that we can store some of those routine
transformations and help reduce the burden on data providers in transforming their data.

## Examples
Here are a few examples from OBIS-USA for taking data from the original format to Darwin Core. Darwin Core term definitions
can be found at:

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
