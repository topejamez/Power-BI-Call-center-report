# Power-BI-Call-center-report

## Table of Contents

- [Project Overview](#project-overview)

- [Data Source](#data-source)

- [Tools](#tools)

- [Data Preparation](#data-preparation)

- [Data Analysis](#data-analysis)

- [Results](#results)

- [Recommendations](#recommendations)



## Project Overview

This report provides a comprehensive overview of call center operations between January and March, including key performance indicators (KPIs) such as call volume, response time, resolution rate, customer satisfaction rating, and agent performance metrics. It analyzes trends, identifies challenges, and offers actionable insights to improve service delivery, enhance customer experience, and optimize operational efficiency.

![Screenshot 2025-04-05 163007](https://github.com/user-attachments/assets/09caabac-5b9b-48d0-9f45-b36251e2db96)

## Data Source

Call center data: The primary dataset used for this analysis is the call_center.xlsx file, which contains detailed information about the call rate of the call center.

## Tools
Excel is the source of the dataset. Power BI was used to clean, transform, format, transform, measure and create the report.

## Data Preparation

In preparing the data, I performed the following tasks: • Deleting redundant columns. • Renaming the columns. • Dropping duplicates. • Cleaning individual columns. • Remove the NaN values from the dataset • Creating new columns using formulas • Creating new measures • Check for some more Transformations. 

## Data Analysis

-- I downloaded the dataset and uploaded the data using the "Get Data" option in Power BI. Then, I utilized the "Transform" option to check for any null values in the dataset.
-- I created new columns to ascribe '1' to 'Y' and '0' to 'N' for both "Answered" and "Resolved" using the formulas below:

~~~Power bi
AnsweredCount = IF('Sheet1'[Answered (Y/N)] = "Y", 1, 0)
~~~
~~~
ResolvedCount = IF('Sheet1'[Resolved (Y/N)] = "Y", 1, 0)
~~~

-- Summing the 1's for both 'Answered' and 'Resolved' gave the number of calls answered and the number of issues resolved.
-- Visuals used include Gauge, slicer, donut chart, bar chart, card, and table.

## Results

The analysis results are summarised as follows:
-- The average satisfaction rating is 3.40 out of 5.0.
-- 81.08% of calls were answered, while 18.92% were not answered.
-- 72.92% of the issues were resolved, while 27.08% were unresolved.
-- The highest answered was recorded in January, while the highest unanswered call was recorded in February.
-- The average speed of answer was recorded to be 67.52 seconds.

## Recommendations

Based on the analysis carried out, I recommend the following actions:

-- Ensure adequate staffing during high-traffic periods like January as seen, to reduce wait times and call abandonment rates.
-- Promote the use of chatbots and FAQs to handle simple queries, freeing agents to handle complex issues.
-- Motivate staff with a reward system for meeting or exceeding performance targets such as resolution rate, satisfaction rating, or low hold time.
-- Maintain an up-to-date internal knowledge base to help agents provide accurate information quickly and consistently, thereby reducing the percentage of unresolved issues.

# Thank you for reading

