# Final-Project-Statistical-Modelling-with-Python

## NOTES(PLEASE READ): 

FOR /notebooks/joining_data.ipynb (For this file, please download it to VSC, It gave an error saying "UNABLE TO RENDER RICK DISPLAY" I worked on this issue with a mentor, she downloaded it to VSC, and it works fine. and she is unsure why github gives this error.)

## Project/Goals

For this project,  it asked us to use three different APIs to get the separate database and join them by using a unique number; I used the station's ID to join the three tables together. For the city bikes, I picked Vancouver since I live here and am more familiar with the city. Later in this project, we need to use the join table to do EDA, data visualization and statistical modelling. 

My goal for the project is to use what I learned for API and Json to collect data, clean my data by using EDA, and finally build the Data Visualisation to explore the data and a regression model.


## Process

Step 1: Explore Citybike API and pick the city. Use API to get latitude, longitude, the number of bikes(free bikes) and the station id, which I use to link my tables later. 

Step 2: Connect to Foursquare API,  and explore the data for each bike station from the city bike table to retrieve information for restaurants. The data I choose to include in my database are the following: restaurant names, ratings, review counts, prices, distance, latitude, and longitude. 

Step 3: Join three tables using the station id from the city bike table. 
EDA - Clean the table to remove duplicates and nulls; Drop the columns I don't need to make the table easier to use. Build Data visualization charts by using seaborn.

Step 4: Build regression models using statsmodels to test the relationship between distance, review counts and ratings. 
      

## Results

R-Square is 0.0004: R-squared reflects the fit of the model. R-squared values range from 0 to 1, where a higher value generally indicates a better fit, assuming certain conditions are met. 
In this output, we can see that the value is only 0.0004. This means that the model needs to be more capable of explaining the patterns in the data.

P - Value: review counts: 0.494 & rating:0.993.

A p-value of less than 0.05 is considered to be statistically significant. 
This regression output shows a p-value for a review count of 0.0494 and a rating is 0.993, which means that the probability of the relationship between the distance does NOT  impact the review counts and ratings. 


## Challenges 

I struggled with API and JSON. I spent 80% of the time correcting my API and JSON.normalize ()codes. Once I got through this part, I finished my project quickly. This is the first time I have heard of  API; I need to study more. 


## Future Goals

Spend more time understanding API better, and I need to improve my coding skills. When I look at the question, I have ideas on how to get it done, but I need to figure out how to write codes to get it done
