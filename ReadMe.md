This project explores the impact of WTO accession on agricultural imports using a Difference-in-Differences (DiD) approach. Focusing on the 36 Article XII WTO member countries that joined after 1995, we compare their agricultural import patterns with a control group of pre-existing GATT/WTO developing members. Our analysis disaggregates the sample into homogeneous clusters, allowing for a detailed investigation of heterogenous treatment effects across different groups. To mitigate issues like autocorrelation in residuals, we employ a bias-corrected FGLS method. The findings reveal varying impacts of WTO accession, with some clusters exhibiting significant changes in trade patterns, while others show little to no effect.

Key methodologies include hierarchical clustering to exclude outliers, KNNMeans for cluster identification, and a rigorous regression analysis to assess the economic effects of accession. This repository contains the code, data, and scripts necessary for replication and further exploration of WTO membership's role in shaping agricultural trade.

#  PROJECT WORKFLOW

This folder has 4 files :

1. *Data_for_Clustering.xlsx*: This is an excel sheet containing the data of the socioeconomic variables as imported from World Bank (World Development Indicators)

2. *Clustering.ipynb*: This contains all the codes regarding the data preparation of the socioeconomic variables for the clustering and the process of clustering.
   - In the first cell the file path of Data_for_Clustering.xlsx has to be given to run the notebook.

3. *Final_Regression_Data.dta*: It contains the final data of the Agri Imports of each country for each year (sourced from FAOSTAT), including the Treatment variable indicator and Cluster assignment. This is the data on which the final regression will be run.

4. *Final_Regression_Agri_Imports.do*: This is the do file containing the codes for the final regression.
   - The file path for Final_Regression_Data has to be provided.
   - The Cluster for which the regression has to be run, needs to be specified, in the relevant area as mentioned in the code.
