# Exploratory Data Analysis of Airbnb data Set
## Table of Contents
* [Introductions](https://github.com/aru20/EDA-Python-Medical-Appointments/tree/main#1-introduction)
* [Data Wrangling](https://github.com/aru20/EDA-Python-Medical-Appointments/tree/main#2-dataset-description)
* [Exploratory Data Analysis](https://github.com/aru20/EDA-Python-Medical-Appointments/tree/main#5-exploratory-data-analysis)
* [Conclusions](https://github.com/aru20/EDA-Python-Medical-Appointments/tree/main#conclusions)

Table of contents
1. Loading libraries and data
1.1 Loading libraries
1.2 The listings and listing details files
2. Data exploration
2.1 Neighbourhoods
2.2 Room types and property types
2.3 Accommodates (number of people)
3. Advice to the municipality of Amsterdam
3.1 Finding possibly illegal hotels
3.2 Unwanted effects of professional hosts
4. Advice to the tourists
4.1 Average daily price per neighbourhood
4.2 Neighbourhood safety
4.3 Review scores location, and location scores versus price
4.4 How to use review scores
4.5 Finding a good host
4.6 Availability over time
4.7 Average price by date
5. Text mining the Review comments

## 1. Introduction
Airbnb is an online platform that allows individuals to rent out their properties, such as apartments, houses, or rooms, to travelers looking for accommodation.The platform connects hosts and guests by providing a user-friendly website and mobile app where hosts can list their available properties, set their own rental prices, and provide details about the accommodations. Guests can search for and book these properties based on their preferences, travel dates, and desired location.Airbnb also offers a review system where hosts and guests can rate and review each other based on their experiences. This helps build trust and transparency within the community and allows both parties to make informed decisions when booking or hosting.
There are many factors which influence the price of a listing. Which is why we aim to find the most important factors that affect the price and more importantly the features that is common among the most expensive listings. This will allow an aspiring AirBnb host to ensure that his listing is equipped with those important features such that he will be able to charge a higher price without losing customers. Moreover, a traveller will also know the factors to look into to get the lowest price possible while having certain features he prefers.
Exploring Airbnb data sets will give us many valuable insights regarding customer behavoiur, booking pattern and most popular destinations and so on.
* Understanding Customer behaviour: 
Some questions we can ask to help us explore the data are:

* What are the features/facilities/ammenities of a property that affect its price?
* What is the demand patterns, seasonal fluctuations, and other factors that affect pricing?
* How we can enhance user experiances?
* What are the popular neighborhoods in SanFransico , and what are the property types that are in high demand?
* 
## 2. Dataset Description: 
This is an Airbnb data set taken from [InsideAirbnb](http://insideairbnb.com/get-the-data/.) We used the Airbnb dataset for SanFransico and analysed the listings in SanFransico. The data is as of 03/06/2023.

### 2.1 Data Dictionary

* availability_365 - number of days that the property was available, within 365
* calculated_host_listings_count - total amount of properties owned by the same host
* host_name - name of the host
* host_id - id number of the host
* id - id number generated to identify the property
* last_review - date of the last review made
* latitude - property latitude coordinate
* license- number of registration, license or permission
* longitude - property longitude coordinate
* minimum_nights - a minimum amount of nights to book
* name - property's name
* neighbourhood - neighborhood; in a more specific way then the next variable; it means a smaller area
* neighbourhood_group - a neighborhood within the 5 that New York has; it is larger than the variable before
* number_of_reviews_ltm - number of reviews that the property received in the last 12 months
* price - price to rent the property (local currency)
* reviews_per_month - amount of reviews received per month
* room_type - the type of property that is offered (private room, shared room, or entire place)
* The above information was taken from [Inside Airbnb Data Dictionary.](https://docs.google.com/spreadsheets/d/1iWCNJcSutYqpULSQHlNyGInUvHg2BoUGoNRIGa6Szc4/edit?pli=1#gid=1322284596)
### 2.2 Data Information
This section will provide basic information about the data.



## 3. Data Wrangling/Data Processing
In this step, we will prepare the data for further analysis. That is, we will clean the data, remove duplicates, identify and impute missing data, and format the data in a standardized format. We will also look for outliers.
The primary goal of this data-wrangling step is to ensure data quality, consistency, and compatibility before proceeding with further analysis.

