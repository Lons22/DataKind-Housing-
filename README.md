In this workstream, volunteers will analyze and visualize housing-related information at the Census tract or other geographic level to identify potential relationships between economic, demographic, and social variables at a designated geographic level. The intent of this workstream is to explore data and identify potential relationships between variables that would identify areas of housing need and housing opportunity.

The first part of this visualization I created a map that highlighted the affordable housing development failures in Orlando. Tha failures don't appear to be clustered in one area. To confirm this, I wanted to do a cluster analysis. I filtered the dataset in Python to failures and selected the relevant attributes of: city, state, zip code, latitude, longitude, number of units, bedrooms and NLM reason. I kept running into issues when analyzing the variables because they were classified as FLOAT-64 so I changed them to INT-64 and removed the ones that could not be changed to an integer (city, state, latitude and longitude). I tried to create a heatmap but I kept running into an issue with NA values. Same with attempting the cluster analysis. If you drop the NA values from the dataset, you are left with an empty data frame. The issue with the NA values must be solved to complete a successful analysis to understand the features of failures.  I was able to create a histogram and found that most failures had between 0- 100 units. 
