# **Brooklyn Pizza Restaurants Analysis**

Date Started: 9/10/2023

# **Project Description:**

- Using an API, I extracted Yelp data and mergeed it with health inspections data for Pizza restaurants in Brooklyn
- By employing hypothesis testing, the objective is to investigate the relationship between elevated inspection scores and the likelihood of restaurants in Brooklyn that serve pizza garnering enhanced reviews on Yelp

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

About NYC Health Inspections data: 
This dataset includes NYC restuarant inpection data for the last three years prior to the most recent inspection and does not include restaurants that go out of business. Letter grading inspections were put on pause beginning March 17, 2020, until July 19, 2021, due to the COVID-19 public health emergency. Modified restaurant inspections occurred during this time. Restaurants are uniquely identified by their CAMIS number. Only restaurants that are currently active as of the date of this extraction are included in the dataset. Establishments with inspection date of 1/1/1900 are new establishments that have not yet received an inspection. These will be excluded from parts of the project.

About YELP data:
I only included YELP data specifically for pizza restaurants in Brooklyn,NY. This helped to focus on a smaller dataset to search for correlation between the inspection scores and ratings. 


# **Data Dictionary**

**DBA**	This field represents the name (doing business as) of the entity (restaurant); Public business name, may change at discretion of restaurant owner

**BORO**	Borough in which the entity (restaurant) is located.;• 1 = MANHATTAN • 2 = BRONX • 3 = BROOKLYN • 4 = QUEENS • 5 = STATEN ISLAND • Missing; NOTE: There may be discrepancies between zip code and listed boro due to differences in an establishment's mailing address and physical location

**BUILDING**  Building number for establishment (restaurant) location

**STREET**	Street name for establishment (restaurant) location

**ZIPCODE**	Zip code of establishment (restaurant) location

**PHONE**	Phone Number; Phone number provided by restaurant owner/manager

**CUISINE DESCRIPTION**	This field describes the entity (restaurant) cuisine. ; Optional field provided by provided by restaurant owner/manager

**INSPECTION DATE**	This field represents the date of inspection; NOTE: Inspection dates of 1/1/1900 mean an establishment has not yet had an inspection

**ACTION**	This field represents the actions that is associated with each restaurant inspection. ; • Violations were cited in the following area(s). • No violations were recorded at the time of this inspection. • Establishment re-opened by DOHMH • Establishment re-closed by DOHMH • Establishment Closed by DOHMH. Violations were cited in the following area(s) and those requiring immediate action were addressed. • "Missing" = not yet inspected;

**VIOLATION CODE**	Violation code associated with an establishment (restaurant) inspection

**VIOLATION DESCRIPTION**Violation description associated with an establishment (restaurant) inspection

**CRITICAL FLAG**	Indicator of critical violation; "• Critical • Not Critical • Not Applicable"; Critical violations are those most likely to contribute to food-borne illness

**SCORE**Total score for a particular inspection; Scores are updated based on adjudication results

**GRADE**	Grade associated with the inspection; • N = Not Yet Graded• A = Grade A• B = Grade B• C = Grade C• Z = Grade Pending• P= Grade Pending issued on re-opening following an initial inspection that resulted in a closure

**GRADE DATE**	The date when the current grade was issued to the entity (restaurant)

**RECORD DATE**	The date when the extract was run to produce this data set

**INSPECTION TYPE** A combination of the inspection program and the type of inspection performed; See Data Dictionary for full list of expected values


# **Methods**

- I used hypothesis testing to find out whether or not there was any correlation between better inspections scores mean better ratings on Yelp. I used Z-scores to help identify any outliers and elimnated them before performing 3 different hypothesis tests. Unfortunately, there was no significant correlation found.

- I used many different visualization methods using matplotlib, seaborn, and pandas. I also included a geospatial visualization summing up the majority of my findings.

# **Inspections EDA**
This visualization shows that the majority of the restaurants in NYC have a good score and are able to remain open

![Distribution of Box Scores for inspections](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/53c31b9b-b282-431a-81f9-1e7a8221b24d)


# **YELP EDA**

This visualization shows the ratings and review counts for Pizza restaurants in Brooklyn

![Boxplot of ratings and review counts](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/75ed7392-6887-48f1-982d-e4e1dd270f2c)

This visualization shows that the majority of Pizza restaurants in Brooklyn are rated between 3.5 and 4.5

![Distribution of Ratings for Pizza](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/76a12cff-936f-4670-ba48-9e6f0ab7db0a)


This visualization shows the review counts for Pizza restaurants in Brooklyn with at least 200 reviews

![Review counts for restaurants](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/4c700f6b-33d1-4ca3-b7dd-143f92fe894c)

# **Model specs**
