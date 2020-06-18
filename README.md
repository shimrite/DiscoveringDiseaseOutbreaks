# DiscoveringDiseaseOutbreaks
This project discover disease outbreaks from news headlines, using names location detection, transforming into geo-locations (coordinates) and classification of these points into groups.  
* This project was built as part of a LiveProject of Manning site.

This project contain the following files:
### 1. GeoNamesAndLocations.ipynb - 
this module extract cities and countries names from each headline (if exist). then we transform every name to its geo-location (using geonamescache library). 
### 2. GeoClusteringByLoc.ipynb - 
this module classifies the discovered lovations into clusters.
### 3. data/headlines.txt - 
the input data file, to be placed under "data" folder.
