# Final-Project-Tableau

## Project/Goals
The purpose of this project was to prepare impactful visualization using Tableau for a given dataset and make a meaningful dashboard to communicate business insights about Airbnb dataset.

## Process
As objectives defined in the project:
- Turned data into easily consumable visual insights, using Tableau
- Created impactful dashboards that can help stakeholders make decisions, based on a business questions
- Communicate insights with the correct visualizations


### 1. Data Connection - Collect/download the dataset to be analyzed and connect in Tableau using Datasource

### 2. Detect Datatypes -
Review data and check if all datatypes are appropriate according to column names. </br>
- Host Id		:Number
- Host Since  	:Date      
- Name 		:String
- Neighbourhood  	:String
- Property Type	:String
- Review Scores Rating (bin) :Number
- Room Type	:String
- Zipcode		:Number (Geographic Role)
- Beds		:Number
- Number of Records: Number
- Number Of Reviews :Number
- Price 		:Number
- Review Scores Rating : Number </br>

Check for null values, duplicate data, invalid or incorrect data. Such data can be easily filtered out in Tableau. </br>

Categorical Features :</br>
Room Type </br>
Beds </br>
Price </br>
Neighborhood </br>
Host Since </br>


### 3. Build Visualization for EDA :</br>
Following slides consist all the visualization.</br>
Find an interesting pattern, trend, outlier, etc. from the data used in the above steps.</br>
Please refer TableauPresentation2AirbnbPaliwalHarshita.pdf in /Presentation directory and Final Tableau Project LHL11.twbx in /Tableau Workbook directory for below described Visualizations</br>

#### - Hostby_season : This graph tells count of units added each year as per season. I have created 'Season' calculated field using 'Host since' date column and divided year into seasons summer,winter,fall,spring

#### - Filter by area,property,room : This graph providescount of units according to property type and room type in each neighbourhood. There are two filters one for property type and one for room type.

#### - Avg Price Map : It is a map to show average price in each zipcode in each neighborhood.

#### - Avg Review Score by NBH : This graph shows neighborhood based on review score rating.

#### - Top Airbnb : This graph shows top Airbnb and their details like neighnorhood, Name, Rating and Price. Here there is a 'Top Airbnb' which can be used select top 10,15 or 20 airbnbs. This might give more airbnbs in the list if they have same price.

#### - Filter by year/quarter/month : This graph shows count of units added as airbnb in each year which can be drilled down to quarter and month for each neighborhood. Here I have created 'Date Calculation' calculated field and 'Date_Parameter' for hierarchy.

#### - Catgeory : This graph gives count of units according to Affordable/Costly/Expensive/Luxury categories based on Price for each neighborhood.

#### - Forecast : For number of units getting added as Airbnb in coming two years and price of airbnb in coming two years.

#### - Cluster : I tried to cluster Variables: Count of Beds, Avg. Review Scores Rating, Count of Number of Records, Count of Review with level of detail : Neighbourhood, Property Type, Room Type and found that given variables significantly affect the cluster based on p values.

#### - Top 10 by Reviews : This graph shows overall top airbnb(with details) based on reviews from each neighborhood

#### - Average price by property type, average price by Room Type and average price by Neighborhood these are straight forward graphs

#### - General Information : it is a map which provides all details about airbnb when we hover on it.

### 4. Create dashboard

#### Performace Dashboard: </br>
It is for Airbnb executive or Host to get trend about how and where Airbnb units are added. </br>
Map shows average price in each zipcode for each neighborhood </br>
Average price by year shows variance in price every year and what would be the average price in coming two years based on historical data </br>
The donut chart shows percentage of total units each neighborhood which clearly shows Manhattan has the maximum airbnbs of total Airbnb in New York City and Staten Island is least favored neighborhood for Airbnb. </br>
Unit added per year forecast predicts how many units will be added in coming years. </br>
Unit count by Year/Quarter/Month tells how many units were added each year or quarter or month which explains Airbnb gained popularity by 2014 as compared to 2008. Also most units were added during June/July when people plan most their vacations. </br>
Unit count by season explains most units are added during Summer and least during Winter. </br>
This dashboard can provide details specific to each neighborhood using filter ‘Neighborhood’ </br>
Date parameter can be used to drill down information by quarter and month. </br>

#### Customer Dashboard : </br>
This dashboard is for customer looking for an Airbnb in a particular neighborhood trying to know Top Airbnb, average price by property type, average price by room type and neighborhood. General information map shows every detail about an Airbnb when we hover on it. </br>

It gives details about Top 10,15 or 20 Airbnbs using filter provide ‘Top Airbnb’. A parameter was created to perform this functionality. </br>
It shows average price for each property type by neighborhood. E.g. average price for apartment in Bronx is $82.47 </br>
It gives average price by room type, e.g. for private room in Queens average price is $72.46 </br>
Average price in Manhattan is $198.47 with average rating as 91.8 </br>
Manhattan is the most expensive neighborhood and Bronx is cheapest one. </br>

### 5. Data Interpretation: </br>
Detect Meaningful keypoints and answer relevant questions observed from visualization.

## Results </br>
I have chosen the Airbnb dataset as I was familiar with the information provided in this and could conclude below observations: </br>
- Manhattan is the most expensive neighbourhood and Bronx is cheapest
- Manhattan has the major share of airbnbs of total Airbnb units available in New York.
- Airbnb gained significant popularity over the years starting from 2008 to 2014.
- Most units were added during Summer season and least during winter season
- Property type ‘Apartment’ has the maximum count in all units added as Airbnb.

## Challenges 
- Tableau automatically does certain aggregations which are not required
- It is a bit difficult to connect each viz and create meaningful interpretation
- Data needs to be formatted for each column
- Tooltip needs to be updated carefully so that it shows correct data with understandable names



## Future Goals </br>
If given more time I will explore more ways to improve visualization and add more insights to the current analysis. </br>
I would like to learn more about animation which can be added in this scenario.
