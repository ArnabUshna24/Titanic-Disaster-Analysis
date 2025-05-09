# Titanic Disaster Analysis



## Overview
This project aims to analyze [Titanic - Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data) dataset and find insights using statistical analysis. It serves the following concerns:

* Retriveing the data from the target location.
* Handling the missing values and outliers (if there is any).
* Performing data visualization.
* Performing basis statistical analyses.


## Data Retrieval
`Titanic - Machine Learning from Disaster` dataset is available on Kaggle. It contains three (3) `.csv` files - `gender_submission.csv`, `test.csv`, and `train.csv`. Among them, `train.csv` file was used for this project. It contains twelve (12) colunmns - `PassengerId`,	`Survived`,	`Pclass`,	`Name`,	`Sex`,	`Age`,	`SibSp`, 	`Parch`, `Ticket`, `Fare`, `Cabin`, and	`Embarked`. `train.csv` file was loaded into a `pandas` dataframe for further analysis.


## Data Cleaning and Manipulation
To find missing values in the dataset, `isnull` function was used. There were 177 missing `Age` values, 687 missing `Cabin` values, and 2 `Embarked` values. For the missing values in `Age` column, it was imputed with the median of the column values, whereas `Cabin` and `Embarked` columns were handled using `notnull` function and mode, respectively. After that, outlier identification was performed and outliers were then capped. However, there were no duplicated records.


## Data Visualizations
<table>
  
  <tr>
    <td align="center"><img src="https://github.com/ArnabUshna24/Titanic-Disaster-Analysis/blob/main/data_visualizations/gender_distribution.png" alt="Distribution of Passengers by Gender" width="300"/></td>
    <td align="center"><img src="https://github.com/ArnabUshna24/Titanic-Disaster-Analysis/blob/main/data_visualizations/age_distribution.png" alt="Age Distribution Histogram" width="300"/></td>
  </tr>
  
  <tr>
    <td align="center"> Fig. 1: Distribution of Passengers by Gender </td>
    <td align="center"> Fig. 2: Age Distribution Histogram </td>
  </tr>
  
  <tr>
    <td align="center"><img src="https://github.com/ArnabUshna24/Titanic-Disaster-Analysis/blob/main/data_visualizations/gender-wise_survival_rate.png" alt="Survival Rate by Gender" width="300"/></td>
    <td align="center"><img src="https://github.com/ArnabUshna24/Titanic-Disaster-Analysis/blob/main/data_visualizations/class-wise_survival_rate.png" alt="Survival Rate by Class" width="300"/></td>
  </tr>
  
   <tr>
    <td align="center"> Fig. 3: Survival Rate by Gender </td>
    <td align="center"> Fig. 4: Survival Rate by Class </td>
  </tr>
  
</table>



## Statistical Analysis
<p><strong>Table 1:</strong> Mean, Median and Mode of 'Fare' and 'Age' Columns </p>
<table border="1" cellspacing="0" cellpadding="5">
  <tr>
    <th align="left"> Columns </th>
    <th align="center"> Mean </th>
    <th align="center"> Median </th>
    <th align="center"> Mode </th>
  </tr>
  <tr>
    <td align="left"> Fare </td>
    <td align="center"> 32.2042 </td>
    <td align="center"> 14.4542 </td>
    <td align="center"> 8.05 </td>
  </tr>
  <tr>
    <td align="left"> Age </td>
    <td align="center"> 29.3616 </td>
    <td align="center"> 28.0 </td>
    <td align="center"> 28.0 </td>
  </tr>
</table>


<p><strong>Table 2:</strong> Gender-wise Survival Rate </p>
<table border="1" cellspacing="0" cellpadding="5">
  <tr>
    <th align="left"> Test Component </th>
    <th align="center"> Result </th>
  </tr>
  
  <tr>
    <td align="left"> Null hypothesis </td>
    <td align="center"> Significant difference in survival rates </td>
  </tr>

  <tr>
    <td align="left"> Significance level (α) </td>
    <td align="center"> 0.05 </td>
  </tr>

  <tr>
    <td align="left"> T-statistic </td>
    <td align="center"> -18.672 </td>
  </tr>

  <tr>
    <td align="left"> P-value </td>
    <td align="center"> 2.28 × 10⁻⁶¹ </td>
  </tr>

  <tr>
    <td align="left"> Decision </td>
    <td align="center"> Reject the null hypothesis </td>
  </tr>

   <tr>
    <td align="left"> Interpretation </td>
    <td align="center"> There is a significant difference in survival rates between males and females on the Titanic </td>
  </tr>
</table>


## Build from Source
Instructions are provided in the `ipynb` file.


If you have any queries, contact me: arnabnushna24@gmail.com
