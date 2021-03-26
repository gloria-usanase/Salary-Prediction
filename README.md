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
<br>
jobId: Unique identifier for each employee 
<br>
salary: Annual salary 
<br>
companyId: Identifier for each company 
<br>
jobType: Position held within the company (CEO, CFO, CTO, Vice President, Manager, Janitor, Senior, or Junior) 
<br>
degree: Doctoral, Masters, Bachelors, High School, or None
<br>
major: field of study 
<br>
industry: field of work 
<br>
yearsExperience: how many years of work experience 
<br>
milesFromMetropolis: miles away the job is from a major city
<br />
<br>
![Dataview1](./img/sampledata1.png) <br /><br>
![Dataview2](./img/sampledata2.png)

## Methodology

1. Exploratory Data Analysis:<br />
Summarized data and created plots for each category as seen in the diagrams below:<br />
Data Summary:<br />
![Plot](./img/summary.png) <br />

Job Type: There is a clear positive correlation between job type and salary. <br />
![Plot](./img/jobtype.png) <br />

Degree: People with higher degrees have higher salaries. <br />
![Plot](./img/degree.png) <br />

Major: Engineering major have higher salaries. <br />
![Plot](./img/major.png) <br />

Industry: Oil and Finance industries have the same salaries and pay better compared to other industries. <br />
![Plot](./img/industry.png) <br />

Years of experience:There is a clear correlation between salary and years of experience. <br />
![Plot](./img/yearsexperience.png) <br />

Miles from metropolis: Salary decreases with distance from major cities. <br />
![Plot](./img/milesfrommetropolis.png) <br />

Heatmap:<br />
![Heatmap](./img/heatmap.png) <br />

2. Model Building and Evaluation:<br />
Created 4 different models then chose the model with the lowest MSE.<br />
- Linear Regression => MSE:384.46 <br />
- Pipeline => MSE:384.46 <br />
- Random Forest Regressor => MSE:367.74 <br />
- Gradient Boosting Regressor => MSE:357.23 <br />
<br />
<br />
   As seen on the image below, the job type janitor has the highest importance meaning lowest salary.<br />
   ![FeatureImportance](./img/featureimportance.png) 
