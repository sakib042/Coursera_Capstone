## Predicting the Possible Location for Opening a Restaurant in Stockholm, Sweden.

##### - by Md. Nazmus Sakib

### 1.Introduction
#### 1.1 Background
In this project, we will try to find an optimal location for a restaurant. Specifically, this report will be targeted to stakeholders interested in opening a Coffee Shop/Restaurant in Stockholm, Sweden.
#### 1.2 Problem
Since there are lots of restaurants in Stockholm we will try to detect locations that are not already crowded with restaurants. We are also particularly interested in areas with no coffee shop in the vicinity. We would also prefer locations as close to the city center as possible, assuming that the first two conditions are met.
#### 1.3 Interest
We will use our data science powers to generate a few most promising neighborhoods based on these criteria. Advantages of each area will then be clearly expressed so that the best possible final location can be chosen by stakeholders.

### 2. Data acquisition and cleaning 
#### 2.1 Data sources
Based on definition of our problem, factors that will influence our decision are:
Sometimes you want bullet points:

* number of existing coffee shop in the neighborhood (including restaurant offer coffee)
* number of and distance to other coffee shop/restaurant in the neighborhood, if any
* distance of neighborhood from city center

We decided to use regularly spaced grid of locations, centered around city center, to define our neighborhoods.
Following data sources will be needed to extract/generate the required information:
*	centers of candidate areas will be generated algorithmically and approximate addresses of centers of those areas will be obtained using Google Maps API reverse geocoding
*	number of coffee shop and their type and location in every neighborhood will be obtained using Foursquare API
*	coordinate of Stockholm center will be obtained using Google Maps API geocoding
