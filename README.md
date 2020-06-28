# DiscoveringDiseaseOutbreaks
This project discover disease outbreaks from news headlines, using names location detection, transforming into geo-locations (coordinates) and classify these points into clusters.  
* This project was built as a LiveProject (Manning).
#Unsupervised#Clusterring#RegularExperssion#Geonamescache#Kmeans#DBSCAN#Basemap

## The project is broken into the following parts:
1. Extracting City and Country Information from News Headlines (data/headlines.txt file attached)
2. Finding Geographic Locations of Headlines (using geonamescach library)
3. Clustering Headlines Based on Location (KMeans, DBSCAN)

## This project contain the following files:
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
### 4. environment.yml -
in order to run this project use the environment.yml file:
> conda env create -f environment.yml

## Results:
![Alt text](LocationsClustersResults.png?raw=true "Title")
