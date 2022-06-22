# Citibike_forecasting

Project name: NYC City Bike Rideshare Study and Forecasting

Project member: Xi Yan & Marissa Ferrighetto 

## Access to final report
[Final report (jupyter notebook)](https://github.com/Nellyan4/Citibike_forecasting/blob/main/Project2-Final.ipynb)

[Recorded presentation in box](https://youtu.be/c303cyhCUzU](https://cmu.app.box.com/s/tg6iev9omnd9144kxvhk0lwzduzx3dfl))

## Key Findings:
1. Our trained models performed better than the baselines for the two research questions
2. The classification models can aid program administrators in deciding which bike types to distribute to a specific start station when they are facing a distribution problem
3. The models can also help them understanding ridership trends by the type of user engagement
4. Understanding these trends can allow them to create user personas to guide marketing decisions and user experience considerations as the program grows


## Implications of Findings:
Democratic state and governors have done sufficient work to increase the minimum wage so that to protect their workers from being harm by the inflation. Yet, due to the unchanged minimum wage in many Republican states, workers in those states are harmed by earning less hourly rate from 1970 and 2020. This needs to be changed in Republican states.

The increases of minimum wage could be beneficial to labor productivity, as exhibited in data. State governors should not be too afraid to increase minimum wage since the increase in labor productivity could substitute the cost for labor.

## Motivation
As Heinz students, studying public policy and information systems, we are interested in how we can apply data science to public problems. We are interested in public transit and commuter patterns through cities. When we saw the expansive data set from New York City’s bike-share system, we were interested in applying machine learning techniques to the data.

## What is the problem?
Increased demand for city bikes since the beginning of the COVID-19 pandemic lead to

**Distribution problem**: There are excess amount of bikes concentrated in some end stations where people generally find no bikes available in many stations. Redistribution is needed to address the supply and demand.

**Business problem**: How to direct increased funding as the bike program continues? Who uses the bike share problem? How can the program build user personas to segment and target users


## Domain & Overview

We plan on applying classification modeling for this project. The classification models can help drive funding decisions and allow stakeholders to better understand their user base.

As we discussed in the lecture, “A Computer Program is said to learn from experience with respect to some class of tasks T and performance measure P, if its performance at tasks in T, as measured by P, improves with E.” In the context of this machine learning project, the T tasks represents the classification modeling, E experience is the training and fitting of the models, and P performance are the results (such as accuracy) of the models.

For this project, we will measure performance based on the different tasks, T. For example, we will compare the accuracy and precision of the classifications.

Our goal is to find a feasible model that can be beneficial to potentially answering the questions that we proposed below. Our objective, for the performance, P, of the models is, to achieve over 50% of accuracy or other relevant metrics when doing a binary classification and over 100/n% when we are doing n numbers classification.

Concisely stated, our goal is to achieve P(T, E+ΔE) > P(T,E).

T: classification modeling

E: training and model fitting

P: accuracy of the models

## Related Work

1. [Citi Bike Struggles to Keep Up With New Yorkers’ Love of Cycling](https://www.nytimes.com/2021/12/02/nyregion/citi-bike-parking-docking-station.html)

  In this article, the author describes the growth of the New York City bike share post-pandemic era and the pain spot of the system. There are demand problems that do not meet the increasing popularity of rideshare and also distribution problems although the Citi bike rideshare system has already deployed hundreds of thousands of bikes, there are situations where users are not able to find bikes at destined bike stops. This implies that a study about the usage of rides to solve the redistribution problem might be urged.

2. [Survey Says: City Voters Support Public Money Invested in Bike Share](https://nyc.streetsblog.org/2021/05/11/survey-says-city-voters-support-public-money-invested-in-bike-share/)

  This article talks about the significance and public support for increasing subsidies and public funding for the New York City rideshare. New York City is the most crowded city in the U.S., and if having as many cars per household as other cities, the traffic situation would become worse. As the article mentioned, “we need to learn more and more into — opening up public spaces, getting out of our cars, focusing more on public transportation. This is the way of the future, unquestionably” This also leaves a question for public transportation developers - how to spend the money most efficiently so that can best serve the public needs of New York City citizens?

3. [New York 25x25 Plan](https://nyc25x25.org/)

  This website is the main page of the advocacy, the New York 25x25 plan. This plan asks mayoral candidates to commit to dedicating 25 percent of the space now designated for vehicles — including 19,000 miles of roads and three million on-street parking spaces — as space for people by 2025 so that New Yorkers might have room to recover from (and thrive after) the COVID-19 pandemic, which has highlighted the city’s lack of equity when it comes to active transportation and green space. 
## Data

### Data Source
We downloaded dataset of [Citi Bike rideshare data](https://ride.citibikenyc.com/system-data) in the Citi Bike website.

### Dataset Description
- The data is stored monthly (total 37 CSV files)
- Each month is a separate CSV file
- Rows: around 50000 for each CSV file (Sum of about 2 million rows)
- Columns: 13
- The data itself is cleaned. It is also expandable to look at the distance between the start station and the end station

### Dataset Features
- Ride ID
- Rideable type (Classic Bike or Electric Bike)
- Started at (MM/DD/YY H:MM:SS)
- Ended at (MM/DD/YY H:MM:SS)
- Start station name
- Start station ID
- End station name
- End station ID
- Start latitude
- Start longitude
- End latitude
- End Longitude
- Member or casual ride (Causal or Member)
