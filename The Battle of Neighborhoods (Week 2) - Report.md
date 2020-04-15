# The Battle of Neighborhoods (Week 1) - Report



**Introduction**

In this week's submission, I have selected to use the city of Toronto and find neighborhoods that would be best suited for a restaurant. This is created in a way to allow a person to get a brief knowledge into who will be the target market for a certain area based on the overall population of that area.



**Business Problem**

Toronto encompasses a geographical area formerly administered by many separate municipalities. These municipalities have each developed a distinct history and identity over the years, and their names remain in common use among Torontonians. Former municipalities include East York, Etobicoke, Forest Hill, Mimico, North York, Parkdale, Scarborough, Swansea, Weston and York. Throughout the city there exist hundreds of 
small neighbourhoods and some larger neighbourhoods covering a few square kilometres.

Toronto's neighborhood is divided into multiple types ranging from Old Toronto to Suburbs to Industrial areas. Toronto also is the most populous city in Canada and has a really diverse population allowing it to become an important destination to a lot of immigrants arriving to Canada. 

This diversity as well as the sheer size of the city itself makes it really difficult for a new business to decide what area would be most suited for their business in such a way that they can maximize their profit without worrying about as less competition as possible.

Thus, thats the idea behind this project as a way to allow new business with some knowledge on where and when to open a new business in an area.



**Data Used**

Based on the problem undertaken, multiple components affect the decision to be taken, some of which are:

    **1.** Any exisiting restaurant in the borough or neighborhood.

    **2.** Age and income of the people visiting these restaurant.

    **3.** Distance to the city centre.

Utilization of **Wikipedia **was used to generate areas centers along with the use of the **Foursquare **API to get the number of restaurant and their types in the areas obtained through the Wikipedia.



**Methodology**

As discussed in the Business problem, the main initiative of the project is to find the best possible location for a restaurant to open to minimize competition and maximize profit.

To achieve the same, we require two data sets, one that provides us with boroughs information in Toronto as well as another that provides us with the age group and population of said areas. To solve the problem, K-Means algorithm was used.

K-Means clustering is a method used for clustering analysis. It is a type of unsupervised learning, which is used when there is unlabeled data present, i.e data without defined categories or groups. The goal of the algorithm is to find groups in the data with the number of groups represented by the variable *K*. The algorithm works iteratively to assign each data point to one of *K* groups based on the features that are provided. Data points are clustered based on feature similarity. The results of the *K*-means clustering algorithm are:

- The centroids of the *K* clusters, which can be used to label new data

- Labels for the training data (each data point is assigned to a single cluster)

Following steps were taken:

- Gathering of data from different sources based on latitude and longitude as well as the types of restaurant in a locality.

- Utilization of K-Means to identify good locations close to center with low number of restauraunt and their types.

- Creation of clusters of location that meet the basic requirements set by the stake-holders. Radius of 500 metres was created to keep a check on other restaurants. 



**Methodology**

*Manipulation of data*

Wikipedia was used to get data for Toronto, Canada. This data was cleaned by removing any and all unnecessary value. 

*Combining different data sources*

Datasets of postal address was combined with dataset of latitude and longitude in a separate dataframe. This new dataframe was visualized using a folium map.

*Usage of Foursquare API*

Foursquare API was utilized to get the data on restaurant in Toronto and filtered the venue for all possible restaurants. Each neighborhood along with the top ten most common venues was identified. 

*Clustering*

K-Means algorithm was used to come up with 5 clusters that were different in Toronto. Identify the clusters & Boroughs/Neighborhoods with Maximum number restaurants and their types.



**Results & Discussion**

Analysis of the data recieved shows that Toronto has a large number of restaurants but there are some areas with with lower amount of restaurants in the city near the city centre. There are 4 boroughs and 39 neighborhoods in the geographical co-ordinates **43.6534817, -79.3839347.** 

Based on the analysis, Cluster 3 has the highest amounts of restaurants than the rest of them. This makes introduction of a new restaurant in that cluster non-feasible due to the amount of restaurants present. Thus, recommended zones should only be taken as a starting point in area selection followed by a detailed analysis to get the full details to get the most out of the area. 



**Conclusion**

The purpose of this coursework was to identify areas in Toronto that have a low amount of restaurants and help new businesses in choosing an optimal location for a restaurant. This was achieved with the utilization of data from Wikipedia as well as the use of the Foursquare API and zones were created to serve as a starting point for further investigation by the stakeholders themselves.

The decision on the optimal location would depend on the stakeholders themselves and will include additional factors besides the one used in this project, such as proximity of location to prime spots like Parks or offices, level of noise and access to the main roads as well as the affordability of real estate along with the socio-economic dynamics of the neighborhoods. Thus, this concludes the project as a whole.




