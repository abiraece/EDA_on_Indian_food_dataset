# EDA_on_Indian_food_dataset

Indian Food Dataset:
Table of Content:
1. Project Introduction
2. Dataset Description
3. Data Preprocessing
4. Data Visualization

Project Introduction:
    Indian cuisine consists of a variety of regional and traditional cuisines native to the Indian subcontinent. 
    Given the diversity in soil, climate, culture, ethnic groups, and occupations, these cuisines vary substantially and use locally available spices, herbs, vegetables, and 
    fruits. Indian food is also heavily influenced by religion, in particular Hinduism, cultural choices and traditions.
    This dataset consists of information about various Indian dishes, their ingredients, their place of origin, etc.
    
Dataset Description:
    name : name of the dish
    ingredients : main ingredients used
    diet : type of diet - either vegetarian or non vegetarian
    prep_time : preparation time
    cook_time : cooking time
    flavor_profile : flavor profile includes whether the dish is spicy, sweet, bitter, etc
    course : course of meal - starter, main course, dessert, etc
    state : state where the dish is famous or is originated
    region : region where the state belongs
    Presence of -1 in any of the columns indicates NaN value.

In Data Preprocessing some of the basic computation are necessary for individual feature analysis. Those are listed as follows:
    As mentioned in the dataset description, there are some Null values in the dataset. First and foremost step is to compute null values present in the Dataset. If null values are
    computed need to impute the null values. In somecase, some special characters or neagtive values may be present in the dataset instead of Null value. 
    As the step of Data Preprocessing all the null values are imputed in this dataset.
    
After null Value imputation, Some of categorical columns are represented as object in the dataset. To perform statstical prediction or to build a model all the features to be encoded.
If the input features are ordinal then proceed with any one listed encoding method : Label encoding, Ordinal Encoding, Replace method
If the input features are nominal then proceed with any one of listed encoding method: One-hot encoding, Frequency Encoding, Target Encoding
In this dataset all different types of encoding are done to convert the categorical column into numerical column for prediction.

Some of Statstical analysis like min,max,IQR,Quantile at 25%,50% and 75%,mean for numerical data and count,unique for categorical data seperately.

Some of Measure of Dispersions like skewness,kurtosis range are also computed to check the ditribution of data.

In Data Visualization, intially boxplot is used to analyse about the outlier. To overcome the Outlier effect capping was done in the dataset.
Different Graphical Analysis made on this dataset and described as follows:
1.Using heatmap, found the correlation between prep_time and cook_time, we conclude that data is more scattered.
2.Based on Falvor_profile analysis performed in different region, we concluded that "West Region" has highest Spicy and Sweet Profile.
3.Based on Diet profile also analysis performed in different region, we concluded that "West Region" has highest profile in Vegetarian.
4.Perfomed analysis on cook_time based on diet,we concluded that for vegetarian diet cook_time will vary based on dishes, 
  but in Non-vegetarian diet cook_time is almost similar for everything.
  
In this Indian Food dataset, Complete EDA Part was done from basic and explained with inferences.
