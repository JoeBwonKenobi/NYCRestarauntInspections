# **Brooklyn Pizza Restaurants Analysis**

![Pizza](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/b411288f-7df4-42d2-9722-3bb830765056)
*I do not own the rights to this photo*


Date Started: 9/10/2023

# **Project Description:**

- Using an API, I extracted Yelp data and mergeed it with health inspections data for Pizza restaurants in Brooklyn.
- By employing hypothesis testing, I attempted to investigate the relationship between elevated inspection scores and the likelihood of restaurants in Brooklyn that serve pizza garnering enhanced reviews on Yelp.
- I used multiple visualization techniques to represent the various aspects of Brooklyn Pizza Restaurants.

# **Data Source:**

https://catalog.data.gov/dataset/dohmh-new-york-city-restaurant-inspection-results

YELP API

# **Necesary links for understanding context within the data**

- https://www.nyc.gov/site/doh/business/food-operators/letter-grading-for-restaurants.page

- https://www.nyc.gov/assets/doh/downloads/pdf/rii/restaurant-grading-faq.pdf


## **Necesary links to run notebooks:**

- #pip install nltk
- #pip install wordcloud
- #nltk.download('stopwords')
- #pip install geopy
- #pip install category_encoders
- #pip install geopandas matplotlib folium
- YELP API key

## **About NYC Health Inspections data:**

This dataset includes NYC restuarant inpection data for the last three years prior to the most recent inspection and does not include restaurants that go out of business. Letter grading inspections were put on pause beginning March 17, 2020, until July 19, 2021, due to the COVID-19 public health emergency. Modified restaurant inspections occurred during this time. Restaurants are uniquely identified by their CAMIS number. Only restaurants that are currently active as of the date of this extraction are included in the dataset. Establishments with inspection date of 1/1/1900 are new establishments that have not yet received an inspection. These will be excluded from parts of the project.

## **About YELP data:**

I only included YELP data specifically for pizza restaurants in Brooklyn,NY. This helped to focus on a smaller dataset to search for correlation between the inspection scores and ratings. 

# **Methods:**

- I used feature engineering to create multiple new columns in the dataset to help gather a more in-depth look into the data.

- I used hypothesis testing to find out whether or not there was any correlation between better inspections scores mean better ratings on Yelp. I used Z-scores to help identify any outliers and elimnated them before performing 3 different hypothesis tests. Unfortunately, there was no significant correlation found.

- I used many different visualization methods using matplotlib, seaborn, and pandas. I also included a geospatial visualization summing up the majority of my findings.

# **NYC Inspections EDA:**

![Distribution of Box Scores for inspections](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/53c31b9b-b282-431a-81f9-1e7a8221b24d)

- The majority of the restaurants score between 5-30, which is a good score and means they're able to remain open after a sucessful initial inspection.

![Average score for pizza restaurants by boro](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/e31e4706-dea6-4f91-b718-2ca8f653d8e8)


![Average Inspection Score for Pizaa Restaurants in each Boro](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/c816f6b4-19e1-45b5-b801-d4427ace5d17)

- The lower the number for the score, the better the restaurant performed on their inspection.
- Brooklyn's average is actulally the worst overall amoungst all the boros.

![Screenshot 2024-01-01 122336](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/f8a10d62-29a0-4ed8-ba9b-8e695291c8af)

- This shows that Brooklyn has the second highest number of restaurants, second only to Manhattan.

# **YELP EDA:**

![Boxplot of ratings and review counts](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/75ed7392-6887-48f1-982d-e4e1dd270f2c)

- As shown above, more reviews does not always mean better ratings on YELP.

![Distribution of Ratings for Pizza](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/76a12cff-936f-4670-ba48-9e6f0ab7db0a)

- This visualization shows that the majority of Pizza restaurants in Brooklyn are rated between 3.5 and 4.5

![Review counts for restaurants](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/4c700f6b-33d1-4ca3-b7dd-143f92fe894c)

- This visualization shows the review counts for Pizza restaurants in Brooklyn with at least 200 reviews.

## **Geospatial Analysis**

[Geospatial Visualization link:](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/blob/main/Brooklyn_Pizza_map.html")

![geospatial viz](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/eccb10aa-f2be-449d-806c-a9f6110663fb)

# **Project Summary**

This project was focused on data involving Pizza Restaurants in Brooklyn, NY.
