# Titanic Disaster Analysis



## Overview
This project aims to analyze [Titanic - Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data) dataset and find insights using statistical analysis. It serves the following concerns:

* Retriveing the data from the target location.
* Handling the missing values and outliers (if there is any).
* Performing data visualization.
* Performing basis statistical analyses.


## Data Retrieval
`Titanic - Machine Learning from Disaster` dataset is available on Kaggle. It contains three (3) `.csv` files - `gender_submission.csv`, `test.csv`, and `train.csv`. Among them, `train.csv` file was used for this project. It contains twelve (12) colunmns - `PassengerId`,	`Survived`,	`Pclass`,	`Name`,	`Sex`,	`Age`,	`SibSp`, 	`Parch`, `Ticket`, `Fare`, `Cabin`, and	`Embarked`. `train.csv` file was loaded into a pandas dataframe for further analysis.


## Data Cleaning and Manipulation
To find missing values in the dataset, `isnull` function was used. There were 177 missing `Age` values, 687 missing `Cabin` values, and 2 `Embarked` values. For the missing values in `Age` column, it was imputed with the median of the column values, whereas `Cabin` and `Embarked` columns were handled using `notnull` function and mode, respectively. After that, outlier identification was performed and outliers were then capped. However, there were no duplicated records.


## Data Visualizations
<table>
  
  <tr>
    <td align="center"><img src="https://github.com/ArnabUshna24/Students-Performance-Analysis/blob/main/data_visualizations/male_female_students_distribution.png" alt="Distribution of Male and Female Students" width="300"/></td>
    <td align="center"><img src="https://github.com/ArnabUshna24/Students-Performance-Analysis/blob/main/data_visualizations/scores_distributions.png" alt="Distribution of Scores" width="300"/></td>
  </tr>
  
  <tr>
    <td align="center"> Fig. 1: Distribution of Male and Female Students </td>
    <td align="center"> Fig. 2: Distribution of Scores </td>
  </tr>
  
  <tr>
    <td align="center"><img src="https://github.com/ArnabUshna24/Students-Performance-Analysis/blob/main/data_visualizations/avg_scores_gender.png" alt="Average Scores by Gender" width="300"/></td>
    <td align="center"><img src="https://github.com/ArnabUshna24/Students-Performance-Analysis/blob/main/data_visualizations/relationship_among_scores.png" alt="Relationship Among Scores" width="300"/></td>
  </tr>
  
   <tr>
    <td align="center"> Fig. 3: Average Scores by Gender </td>
    <td align="center"> Fig. 4: Relationship Among Scores </td>
  </tr>
  
</table>
