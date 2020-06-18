# DiscoveringDiseaseOutbreaks
This project discover disease outbreaks from news headlines, using names location detection, transforming into geo-locations (coordinates) and classify these points into clusters.  
* This project was built as part of a LiveProject of Manning site.
#unsupervised#clusterring#regularExperssion#geonamescache#kmeans#DBSCAN#basemap

This project contain the following files:
### 1. GeoNamesAndLocations.ipynb - 
this module extract cities and countries names from each headline (if exist). 
then we transform every name to its geo-location (using geonamescache library). 
### 2. GeoClusteringByLoc.ipynb - 
this module classifies the discovered geo-locations into clusters.
the clusterring is done using two models:
sklearn.cluster.KMeans - run itereatively on K=[1:10] and analyze inertia_values and silhouette_score
sklearn.cluster.DBSCAN - tested on different parameters as well.
once the points are clustered we visualize them on the world map (using mpl_toolkits.basemap.Basemap)
### 3. data/headlines.txt - 
the input data file, to be placed under "data" folder.
