# Opening-an-Italian-Restaurant-in-Atlanta

Atlanta is the capital and most populous city in the U.S. state of Georgia. With an estimated 2018 population of 498,044, it is also the 37th most-populous city in the United States. The city serves as the cultural and economic center of the Atlanta metropolitan area, home to 5.9 million people and the ninth largest metropolitan area in the nation. 

## Business Problem

As a high populated city, Atlanta is an excellent place to start a new business, specially a restaurant. As part of this project we are interested in find the best locations in Atlanta for open an Italian restaurant in order to increase the investors profits. We want to focus on areas that are not full of restaurants, but also accesible and with a population who like this kind of places.

## Data

For our data we are taking into account the following:

* Number of restaurants in the location
* Number of Italian restaurants

For the data collection we  look in a radius of 15 km from the center of Atlanta. We look for the all the Italian places not only the restaurants. We use the word Italian as search query.

* We use the Foursquare API to obtain the data related to the Italian places in Atlanta. 
* We use Nominatim API to obtain the coordinates of the venues.

## Methodology

We use GitHub  repository as a database. We collect all the data and saved into a Pandas Dataframe which we have to filtered to keep only the features with the relevant information to our study. As we set a radius of 15km, we obtain also some venues out of the limits of Atlanta and we eliminate them, obtaining a new data frame.
We have some categories like 'Boutique' that are totally out of the scope of our problem, in fact we are only interest in categories like 'Italian Restaurant' and 'Pizza Place'. Also, we have one NaN values and we are going to include the correct value manually. We used python folium library to visualize the location of the places on a map ofAtlanta.  We used latitude and longitude values to get the visual.
We used unsupervised learning K-means algorithm to cluster the places and find zones to place our restaurant. K-Means algorithm is one of the most common cluster method of unsupervised learning. We used 3 clusters, and obtain the merged table with cluster labels for each place.

## Results

We obtain a map of Atlanta with the places of our study divided by clusters:


