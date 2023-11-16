# NYC Restaraunt Inspections Project

Date Started: 9/10/2023

# **Project Description:**

- Find Trends and patterns and use machine learning to make predictions of which restaurants will have a secondary inspection and for what violations.
- Use the 'future' inspections in the dataset to predict when a vist or secondary visit wil occur.
- Compare the inspection data with yelp reviews and use hypothesis testing to determine if better scores on inspections make an impact on wether or not a restaurant recives good reviews from YELP
- .
# **Data Source:**

https://catalog.data.gov/dataset/dohmh-new-york-city-restaurant-inspection-results

## **Necesary links to run notebooks:**

- #pip install nltk
- #pip install wordcloud
- #nltk.download('stopwords')
- #pip install geopy
- YELP API key

About NYC Health Inspections data: 
This dataset includes NYC restuarant inpection data for the last three years prior to the most recent inspection and does not include restaurants that go out of business. Letter grading inspections were put on pause beginning March 17, 2020, until July 19, 2021, due to the COVID-19 public health emergency. Modified restaurant inspections occurred during this time. Restaurants are uniquely identified by their CAMIS number. Only restaurants that are currently active as of the date of this extraction are included in the dataset. Establishments with inspection date of 1/1/1900 are new establishments that have not yet received an inspection. These will be excluded from parts of the project.




Add context here

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

# **EDA**

![Cuisine Scores](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/6bb86493-42c0-48ef-94ba-d2d337ba32af)

# **More EDA**

# **Model specs**

**Link to interactive geospacial:**

# **Top Words for violation descriptions**
![Top words for violation descriptions](https://github.com/JoeBwonKenobi/NYCRestarauntInspections/assets/117705408/624196ad-9e9f-446d-ac1a-24a6e793254a)





