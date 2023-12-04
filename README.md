# Life-Expectancy-Report-With-Power-BI

## Table of Content
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools Used](#tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Individual Visuals (Part of Report)](#individual-visuals-part-of-report)
- [The Dashboard](#the-dashboard)
- [Result and Findings](#result-and-findings)
- [Recommendation](#recommendation)
- [Limitation](#limitation)
- [Reference](#reference)



### Project Overview

Analyze the given life expectancy Dataset and generate a report with the following insights: Total number of Counties, Average Life Expectancy, Average Population, Average GDP, Total Expenditure, Top 10 GDP by Countries, Yearly Average Life Expectancy, Country Analysis based on Population, and Life Expectancy by County.

### Data Source

Quantum Analytics NG, a data consultant/business and training school

### Tools Used

Microsoft Power Business Intelligence

### Data Cleaning and Preparation

The Dataset has 22 Columns and over 1 million rows. When I did a close study I discovered the dataset was not 100% valid, though zero error but has lots of empty rows.

Columns like Country, Year, Status, Life_Expectancy, Adult_Mortality, Infant_Death, and many more exist in the Dataset.

I started by cleaning the Dataset by replacing the “null” value with a number zero (0) in the Life_Expectancy Column — replace null Values with 0, and Rounded all figures to 1 decimal point.

How?

I simply highlighted the Column header, right-click on it, and went to “Replace Values” see image below.

![Screenshot_118](https://github.com/Solution92/Life-Expectancy-Report-With-Power-BI/assets/144762124/fc8b5216-05d6-420a-a803-dc2b6663318f)

I also transformed the data using the same process but this time I chose “Transform” — “Round” — “Round Up/Down” as the case may be. Other 

This was the process taken to make sure the Dataset was transformed for the report.

### Exploratory Data Analysis

I created the following different measures and insights under the DAX table and as required.

- Total Number of Countries
- Average Life Expectancy
- Average Population
- Average GDP
- Total Expenditure
- GDP by Countries (Top 10)
- Average Life Expectancy by Yearly
- The sum of Population by Country
- The sum of Life Expectancy by Country

### Data Analysis
~~~
- Total Number of Countries: Total No. of Country = DISTINCTCOUNT(‘Life Expectancy’[Country]) = 193

- Average Life Expectancy: AVG. Life Expectancy = AVERAGE(‘Life

- Expectancy’[Life_Expectancy]) = 68.99

- Average Population: AVG Population = AVERAGE(‘Life Expectancy’[Population]) = 9.92M

- Average GDP: Average GDP = AVERAGE(‘Life Expectancy’[GDP]) = 6.34K

- Total Expenditure: Total Expenditure = SUM(‘Life Expectancy’[Total_Expenditure]) = 16.10K
~~~
### Individual Visuals (Part of Report)

GDP by Countries (Top 10)

![Screenshot_119](https://github.com/Solution92/Life-Expectancy-Report-With-Power-BI/assets/144762124/d3f6839e-8d36-446f-b13d-1e2e5178ceb1)

Average Life Expectancy by Yearly

![Screenshot_125](https://github.com/Solution92/Life-Expectancy-Report-With-Power-BI/assets/144762124/d686bbae-fdfa-4947-ad70-a46b54c8e6cc)

The sum of Population by Country

![Screenshot_121](https://github.com/Solution92/Life-Expectancy-Report-With-Power-BI/assets/144762124/f068ca60-d039-483c-b5cf-8d8ca607551c)

The sum of Life Expectancy by Country

![Screenshot_122](https://github.com/Solution92/Life-Expectancy-Report-With-Power-BI/assets/144762124/1e08cb96-b78b-4117-81c9-d2ea836226e9)


### The Dashboard

![Screenshot_124](https://github.com/Solution92/Life-Expectancy-Report-With-Power-BI/assets/144762124/0eb88bfd-5952-454a-9375-1af545ffea85)


### Result and Findings

- India accounted for 23.13% of Sum of Population.  Across all 193 Countries, the Sum of Population ranged from 0 to 6,743,483,055.  

- At 71.62, 2015 had the highest AVG. Life Expectancy was 7.29% higher than in 2000, which had the lowest AVG. Life Expectancy at 66.75. Across all 16 Years, AVG. Life Expectancy ranged from 66.75 to 71.62.

- Switzerland accounted for 4.93% of Sum of GDP.  Across all 193 Countries, the Sum of GDP ranged from 0 to 917,805.90.    

### Recommendation

- Based on the findings, it is notable that India contributes significantly to the overall population, while Switzerland has a substantial share of the total GDP. 
- The variation in average life expectancy across the years emphasizes the importance of analyzing trends over time. Understanding these demographic and economic patterns can guide policies and interventions to address disparities and promote well-being. 
- Further exploration of specific factors influencing life expectancy and GDP in India and Switzerland would provide valuable insights for targeted strategies and improvements.

### Limitation

- The table provides key insights into the population, life expectancy, and GDP trends; however, it lacks information on specific factors influencing life expectancy and GDP variations. 
- The absence of demographic details or health indicators limits a comprehensive understanding of the observed patterns. 
- Additionally, the table does not address potential correlations or causal relationships between variables, hindering a deeper analysis. 
- It would be beneficial to include contextual information or external factors that might influence the observed trends for a more nuanced interpretation. 
- Lastly, without a breakdown by age groups or regions, the table may overlook disparities within countries, impacting the accuracy of policy recommendations.

### Reference

[Quantum Analytices](www.quantum.com) can be contacted for a sample of this dataset.




