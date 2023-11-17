# Recipes_Reviews_Data_Analysis
This is a data analysis project that explored the recipes and reviews data set from food.com. In this project, we asked whether recipes with more or less ingredients varied in their ratings. This project was completed for DSC 80 at UCSD by Aishwarya Ramesh and Sai Poornasree Balamurugan.

## Introduction 
Everyone likes food, and a great way to learn to make new recipes nowadays is online. However, not everyone has the time or money to make recipes that are more intensive and require more ingredients. Yet, these recipes are often quite delicious and fun to make as well. 

We worked with two datasets from food.com, a website where people post and review recipes. RAW_recipes was a dataset of recipes from food.com and aspects of their preparation, including prep time, number of ingredients, number of steps, nutritional value, etc. It had 83,782 rows with each row representing a unique recipe. The second dataset we worked with was RAW_interactions, which was a dataset that contained reviews and ratings for the recipes in RAW_recipes. Ratings were from 0-5 stars. It had 731,927 rows each represeting a review of a recipe. 

With this data, we sought to ask the question of whether the ratings of recipes that used higher numbers of ingredients were significantly different from those that used a lower number of ingredients. 

The two datasets were later merged, but the columns we used were the `rating` column from RAW_interactions, which we later turned into `avg_rating` by finding the average rating for each recipe, and the `n_ingredients` column from the RAW_recipes dataset.  

## Cleaning and EDA 
In the first step of our cleaning and EDA process, we left merged the two datasets. We merged the RAW_interactions dataset on the RAW_recipes dataset using the `recipe_id` from the RAW_interactions dataset and `id` from the RAW_recipes dataset, both of which are unique identifiers of a recipe. 

In the merged dataset, `recipes_merged`, we filled all rating of 0 with np.NaN. One reason why we may have done this is 

## Assessment of Missingness

## Hypothesis Testing