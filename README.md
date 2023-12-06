# Crime_Clusters
Segmentation of neighbourhoods based on reported crimes

INTRODUCTION

This is unsupervised machine learning with clustering. The data used was obtained from data.police.uk, and it contains records of crimes reported in the West Midlands region of the UK over 1 year (July 2020 to July 2021). The town of interest in the region was Coventry, and the aim was to segment neighbourhoods (referred to as Lower Layer Super Output Area [LSOA]) in the Coventry area based on their crime rates.

DATA COLLECTION AND PROCESSING

A dataframe was created by merging the various csv files that contained the data. Columns of interest were selected, and missing values were dropped as they were very few (< 0.0001%). The data was explored with visualizations. Thereafter, data collected in the Coventry area was filtered out, and the categorical variables were converted to numerical. Due to the large variance of the features, the data was normalized.

 
CLUSTERING

Both hierarchical and k-means clustering were initially tested on the data; hierarchical performed better and was fitted to the data. Cluster labels were generated. Dimensionaluty reduction with principal component analysis was performed in order to visualize the clusters. Barplots were used to examine the characteristics of the clusters.

RESULTS

The lowest and highest numbers of crimes in the West Midlands region were reported in February 2021 and July 2021, respectively.
Violence and sexual offences	was the commonest crime category, while theft from the person was the least common.
Birmingham had the highest number of reported crimes (about 4 times as much as Coventry, which is the area of interest in this aanalysis).

There were four clusters in the Coventry dataset.

Cluster 0: This is the cluster with the second-highest crime rates in all categories apart from vehicle crime (in which it is surpassed by Cluster 1), and 70.5% of the LSOAs in Coventry are in this cluster.

Cluster 1: It has the second-lowest crime rates in all categories part from vehicle crime (in which it surpasses Cluster 0), and contains 21.5% of the LSOAs in Coventry.

Cluster 2: Crime is almost non-existent in this cluster. Criminal damage, other theft, and other crime are the crime categories that had significant numbers of reports in this cluster, thought the rates are still the lowest of all the clusters'. LSOAs in this cluster appear to be the safest places to live in if crime rate is the metric. Only 1.5% of the LSOAs are in this cluster.

Cluster 3: This cluster is characterized by the highest crime rates in all categories. LSOAs in this cluster need to be prioritized for crime control. About 6.5 of the LSOAs are in this cluster.

