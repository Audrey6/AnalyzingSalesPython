# Analyzing Data with Python Case Study: Retail Sales
Using a retail sales dataset from Kaggle, we'll inspect, clean, transform and model data to draw useful information and conclusions that support certain decision making. The dataset consists of 1000 unique values containing customer sales, gender, product type, and profits.

## Description
This analysis aims to answer the following questions:

1. What is the age distribution of the customers?
2. What was the most profitable year/month?
3. Which category generates the most profit?
4. Which Gender generates more revenue?
5. Is there any correlation between the customer's age or gender and revenue?
   
Given these answers, we can aim to make a decision on where to focus our attention to draw in even more revenue.

## Getting Started
### Dependencies
* Python/IDE

### Installing
* https://docs.jupyter.org/en/latest/install/notebook-classic.html
  
### Executing the Program
* Save retail sales dataset to desginated file path
* Install correct libraries and packages found in the script
* Change read csv to correct file path

## Understanding the Data
After importing the dataset, it is important to understand the data you're working with and all the unique values.
![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/129ec7e4-7b52-4de7-8c2e-d9614aeaf39d)
![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/d24e7473-da47-4ba7-a9f1-e03013d7bba8)
We're working with 1000 unique rows with 11 columns (12 columns after we clean/transform the data).

## Data Cleaning
The data was mostly clean, however I made some necessary changes for readbaility and proper code intake.
I first replaced the column name spaces with underscores:

![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/b179e572-6554-4ad5-a809-d23263e3bf42)

Then I converted the date column into a datetime object in order to extract the day, month, and year into components. This then allowed me to convert the numbered months into a string for plotting readability:

![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/7c916c0a-e5e4-44c0-bf99-1088bbba258c)


The last transformation I did was add a new column for age groups so I can easily categorize the groupings for analysis later on:

![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/5de9ae9d-f022-4960-9f9e-e4fb86e2d6bf)

## Data Analysis
The first thing I did was figure out which age group produces the most revenue. To do this I used a pie chart to show the age distribution and their percentage of revenue contribution in the dataset. We see that adults are over half the population and youths provide the smalled contribution. We can interpret reasons such as, adults have more spending power and money.

![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/de03a175-900f-464d-9a97-a3a7e32250d6)

I then wanted to figure out the gender distribution, so I created another pie chart to display the percentage of Males and Females. We can see that the genders are almost equal so there shouldn't be much of a correlation within gender in this dataset.

![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/b15bccc5-29f3-4966-83d9-df9e7d038b9a)

Next, I wanted to show a chart that displays the profit sum per year. Looks like 2023 has done over 400,000 in sales and 2024 has barely any in comparison. Since this barely gives us much detail other than 2023 being a majority of the data and a great year in sales, I took it one step further to present the profits generated per month into a chart. We can see that September provided around 23,000 in sales as the lowest profited month and May provided around 53,000 in sales as the highest profited month. 

![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/ccedc8c1-a548-4842-97cb-bb15dc211b57)

Next, I wanted to see the generated revenues per category. In a pie chart, we can see that all three categories are close in sales, however, electronics has just a bit more. 

![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/45144485-a249-4b7a-b45a-0bcc492d19c9)

Now we can take it one step further and see if these charts and columns have a correlation between each other. To do this, I made a heat map to display correlations between columns.

![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/15eaa6a3-2c9a-4a23-8fa6-1270165e7bad)

We can also run a correlation chart for further insight:
![image](https://github.com/Audrey6/AnalyzingSalesPython/assets/34180394/aab4c18f-9642-4d6a-b4b1-2d56eec8f239)


## Summary
In conclusion, the dataset provides a good avenue to practice data analysis skills with python. My code targets all the analysis questions found at the beginning of this document and can provide us with a deeper insight as to what and who are creating retail sales and if taken a few steps further, we can potentially target these avenues to reach bigger revenues.
