# Data Engineering Capstone Project

## Overview
The purpose of the data engineering capstone project is to give you a chance to combine what you've learned throughout the program. This project will be an important part of your portfolio that will help you achieve your data engineering-related career goals.

In this project, you can choose to complete the project provided for you, or define the scope and data for a project of your own design. Either way, you'll be expected to go through the same steps outlined below.

## Dataset used for this project

**I94 Immigration Data:** This data comes from the US National Tourism and Trade Office. A data dictionary is included in the workspace. This is where the data comes from. There's a sample file so you can take a look at the data in csv format before reading it all in. You do not have to use the entire dataset, just use what you need to accomplish the goal you set at the beginning of the project.
**Airline Tweets Data:** This data comes from Kaggle: https://www.kaggle.com/crowdflower/twitter-airline-sentiment. This data shows a sentiment analysis job about the problems of each major U.S. airline. Twitter data was scraped from February of 2015 and contributors were asked to first classify positive, negative, and neutral tweets, followed by categorizing negative reasons (such as "late flight" or "rude service").
**US Border Crossing Data:** This data also comes from Kaggle:https://www.kaggle.com/akhilv11/border-crossing-entry-data. It shows the records of immigrants who come to US, and the border they will pass, and the relative information.

## Use Case

In this project, I would like to create a 4 dimension table which includes the 3 dataset and their dimensions. And one fact table which can be used by analysts when they want to know the following questions:
- How many visitors/visits entered in US in 2016?
- In which month there were most visitors?
- Which airport accepted most visitors?
- Which state was most popular destination for visitors?
- Which gender and age were most frequent showed among the visitors?
- Which transportation mode was most popular?
- Which airline was most popular?
The analyst can also combine with dimension tables to answer the following questions:
- What were sentiments for the airlines?
- Which airline had most negative comments?
- Which airline had most positive comments?
- Which border had most immigrants crossed?
- What was the most popular transportation measure to cross US border?
- Which states had most entries?


## Project Instructions
To help guide your project, we've broken it down into a series of steps.

### Step 1: Scope the Project and Gather Data
Since the scope of the project will be highly dependent on the data, these two things happen simultaneously. In this step, you’ll:

Identify and gather the data you'll be using for your project (at least two sources and more than 1 million rows). See Project Resources for ideas of what data you can use.
Explain what end use cases you'd like to prepare the data for (e.g., analytics table, app back-end, source-of-truth database, etc.)

### Step 2: Explore and Assess the Data
Explore the data to identify data quality issues, like missing values, duplicate data, etc.
Document steps necessary to clean the data

### Step 3: Define the Data Model
Map out the conceptual data model and explain why you chose that model
List the steps necessary to pipeline the data into the chosen data model

### Step 4: Run ETL to Model the Data
Create the data pipelines and the data model
Include a data dictionary
Run data quality checks to ensure the pipeline ran as expected
Integrity constraints on the relational database (e.g., unique key, data type, etc.)
Unit tests for the scripts to ensure they are doing the right thing
Source/count checks to ensure completeness

### Step 5: Complete Project Write Up
What's the goal? What queries will you want to run? How would Spark or Airflow be incorporated? Why did you choose the model you chose?
Clearly state the rationale for the choice of tools and technologies for the project.
Document the steps of the process.
Propose how often the data should be updated and why.
Post your write-up and final data model in a GitHub repo.
Include a description of how you would approach the problem differently under the following scenarios:
If the data was increased by 100x.
If the pipelines were run on a daily basis by 7am.
If the database needed to be accessed by 100+ people.