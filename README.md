# Salary-Prediction

## Table of contents

- [Purpose](#Purpose)
- [Technologies](#technologies)
- [Dataset](#dataset)
- [Methodology](#methodology)

## Purpose

This project is examine a set of job postings with salaries and then predict salaries for a new set of job postings.

## Technologies

Python

## Dataset

The dataset used has the following columns:
<br>
*jobId:* Unique identifier for each employee 
<br>
*salary:* Annual salary 
<br>
*companyId:* Identifier for each company 
<br>
*jobType:* Position held within the company (CEO, CFO, CTO, Vice President, Manager, Janitor, Senior, or Junior) 
<br>
*degree:* Doctoral, Masters, Bachelors, High School, or None
<br>
*major:* field of study 
<br>
*industry:* field of work 
<br>
*yearsExperience:* how many years of work experience 
<br>
*milesFromMetropolis:* miles away the job is from a major city
![Dataview1](./img/sampledata1.png) <br />
![Dataview2](./img/sampledata2.png)

## Methodology

1. _Exploratory Data Analysis:<br />
Summarized data and created plots for each category as seen in the diagrams below:<br />
Data Summary:<br />
![Histogram](./img/summary.png) <br />

Job Type:<br />
![Histogram](./img/jobtype.png) <br />

Degree:<br />
![Histogram](./img/degree.png) <br />

Major:<br />
![Histogram](./img/major.png) <br />

Industry:<br />
![Histogram](./img/industry.png) <br />

Years of experience:<br />
![Histogram](./img/yearsexperience.png) <br />

Heatmap:<br />
![Histogram](./img/heatmap.png) <br />

2. _Model Building and Evaluation:<br />
Created 4 different models then chose the model with the lowest MSE.
- Linear Regression => MSE:384.46 <br />
- Pipeline => MSE:384.46 <br />
- Random Forest Regressor => MSE:367.74 <br />
- Gradient Boosting Regressor => MSE:357.23 <br />
   As seen on the image below, the job type janitor has the highest importance meaning lowest salary.<br />
   ![FeatureImportance](./img/featureimportance.png) 
