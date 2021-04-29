# Customer Segmentation
## Table of Content
  - [Project Overview](#projectoverview)
  - [Data Description](#datadescription)
  - [Technical Overview](#technicaloverview)
  - [Results](#results)
  
***

<a id='projectoverview'></a>
## Project Overview

In this project, customers' demographical data of an E-commerce online shop has been analyzed in order to perform Customer Segmentation.
This project aims to help the marketing department come up with specific advertisment strategy according to the sharing features of each customer group in order to more effectively 
target each group.

This project is divided into five steps:

1. `Exploratory data analysis` in this part, statistical description examines the various statistical values of the seven variables of the dataset, and by using Pearson Correlation 
method and heatmap, a clear correlation among seven variables was directly explored. 

2. `Feature Scaling` in this part, by using class 'StandardScaler' to standardize the original dataset.

3. `Hierarchical Clustering` in this part, by using 'dendrogram' method found the optimal number of cluster as four.

4. `K-Means Clustering` in this part, by using the 'elbow' method found the optimal number of clusters also as four and each cluster was labeled based on the sharing features of each 
cutomer group. However, the visualization of the four segments by choosing two strongly correlated features as two dimensions could not clearly sepearte the four segments. Hereby, 
though K-means did a decent job the result is far from perfect.

5. `Principle Component Analysis(PCA)` in this part, by applying PCA method each variance ratio was calculated and a line chart shows the cumulative explained variance against the number
of components chosen. According to the rule of thumb, 3 components were chosen to keep 80% of the variance. Lastly, the original dataset with seven dimensions was transformed to 3
dimensions.

6. `K-Means clustering with PCA` in this part, the transformed dataset with three components was segmented using K-Means method again and still got the result as four clusters which
were labeled by the same names used in 'K-Means clustering'. Lastly, by plotting a scatterplot choosing the most two important Components 1&2 the four segments("Well-off", "Standard", 
"Fewer opportunities", and "Career focused" were clearly seperated.

<a id='datadescription'></a>
## Data Description

The data has been provided by internship project and the actual values were revised to some extent for privacy. The dataset contains one data file with customers' seven kinds of demographical features 
and one description file. The description files have information about the features and their explanation.

<a id='technicaloverview'></a>
## Technical Overview

The project has been divided into various steps which include:
* Data Exploration and Manipulation
* Feature Scaling
* Hierarchical Clustering by dendrogram
* K-Means Clustering by k-means++
* Dimensionality Reduction by PCA
* Unsupervised Learning
* Visualization by matplotlib and seaborn
* Data Export 

<a id='results'></a>
## Results

The results have been clearly documented in the Jupyter Notebook. Please refer [Customer Segmentation Project Workbook.ipynb](Customer_Segmentation_Project_Workbook.ipynb) as well as the visualization result of the four customer segmentation showed as below:

![](/images/Customers' Four Segmentation.png)
