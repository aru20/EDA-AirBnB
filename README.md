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
3.2 Unwanted Effects of professional hosts
4. Advice to the tourists
4.1 Average daily price per neighborhood
4.2 Neighbourhood safety
4.3 Review scores location, and location scores versus price
4.4 How to use review scores
4.5 Finding a good host
4.6 Availability over time
4.7 Average price by date
5. Text mining the Review comments

## 1. Introduction
Airbnb is an online platform that allows individuals to rent out their properties, such as apartments, houses, or rooms, to travelers looking for accommodation.The platform connects hosts and guests by providing a user-friendly website and mobile app where hosts can list their available properties, set their own rental prices, and provide details about the accommodations. Guests can search for and book these properties based on their preferences, travel dates, and desired location.Airbnb also offers a review system where hosts and guests can rate and review each other based on their experiences. This helps build trust and transparency within the community and allows both parties to make informed decisions when booking or hosting.
There are many factors that influence the price of a listing. This is why we aim to find the most important factors that affect the price and, more importantly, the features that are common among the most expensive listings. This will allow an aspiring Airbnb host to ensure that his listing is equipped with those important features such that he will be able to charge a higher price without losing customers. Moreover, a traveler will also know the factors to look into to get the lowest price possible while having certain features he prefers.
Exploring Airbnb data sets will give us many valuable insights regarding customer behavior, booking pattern, and most popular destinations, and so on.

* #### Understanding Customer behavior:
  By analyzing Airbnb reservation data, we can get insights into customer preferences, booking patterens and behaviour. This information will help us to understand what attracts     
  guests, their booking habits, popular locations, and factors that influence their decissions making process.This insights will help us to establish marketing strategies, pricing 
  decisions and property management practices.
* #### Optimizing pricing and revenue management:
  By analyzing the reservation data we will be able to identify the demand pattenrns, seasonal fluctions, and other factors that affect the priceing. By understanding the market 
  dynamics, we can optimizeour pricing strategy maximize revenue and occupency rates. The host may maxmize the revenue by adjusting price based on demands,seasonality  or adding some   on demand amenities. 
* #### Enhancing Guest Experiances:
  By analyzing the reviews and feedback we can get valuable informationsregarding guests preferences.By making adjustments based on feedback to ensure guest satisfaction and increase 
  positive reviews.
* #### Identify market trends:
  By analyzing the reservation data, we can identify popular neighbourhoods, high demand property type. This will help the host to make informed decission regarding property 
  investments and targeting specific market segments.
* #### Operational efficiency and resource allocation:
  Analyzing reservation data can help us optimize our operations and resource allocation. By identifying peak booking periods, we can allocate staff and resources accordingly, 
  ensuring smooth operations during busy times.
* #### Fraud detection and risk mitigation:
  Analyzing reservation data can help us to identify potential fraudulent activities or suspicious behavior. By monitoring patterns and anomalies in the data, we can detect and 
  mitigate risks associated with fraudulent bookings, unauthorized guests, or property damage. This can help you ensure the safety and security of your properties and guests.

In our exploratory analysis we will focous on the below questions.

* What are the features/facilities/amenities of a property that affect its price?
* What are the demand patterns, seasonal fluctuations, and other factors that affect pricing?
* How we can enhance user experiences?
* What are the popular neighborhoods in SanFransico, and what are the property types that are in high demand?

## 2. Dataset Description: 
This is an Airbnb data set taken from [InsideAirbnb](http://insideairbnb.com/get-the-data/.) We used the Airbnb dataset for San Francisco and analyzed the listings in SanFransico. The data is as of June 3, 2023.

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

