# Overview
Food production is one of the most significant contributors to environmental degradation, including issues such as climate change, water scarcity and biodiversity loss. The agricultural sector's environmental footprint varies widely across different food products, farming methods and geographical locations. Understanding the environmental impacts of food production is essential for developing more sustainable practices, reducing ecological footprints and making informed policy and consumer choices. 

This project focuses on analysing the environmental impact of food production, with an emphasis on key metrics such as carbon emissions, water usage, land use and biodiversity loss. By leveraging data on food production and environmental factors, this analysis aims to uncover patterns and provide actionable recommendations for more sustainable food systems. 

The goal of this project is to assess the environmental impact of food production at both macro and micro levels and propose data-driven insights to mitigate the negative effects of food production on the environment. This will help policymakers, environmentalists, food producers and consumers make more informed decisions that support sustainability.

## Crisp DM Framework 

The analysis followed the CRISP-DM methodology, which includes the following stages:

Business Understanding

a. Define the project objectives and business goals.

b. Identify key questions that need to be answered. 

Data Understanding 

a. Collect data from various sources.

b. Explore the data (e.g., summary statistics, missing values, patterns).

c. Identify potential issues like inconsistencies, duplicates and outliers

Data Preparation

a. Clean and preprocess the data.

b. Handle missing values and inconsistencies.

c. Transform data into the right format for analysis.


Analysis and Visualisation

a. Exploratory Data Analysis.

b. Confirmatory Data Analysis.

Recommendations

### 1. Business Understanding

The objectives were defined below, followed by the formulation of analytic questions to guide the analysis.

Objectives 
- Assess the environmental impact of food production: Analyse the environmental impact of these different food products based on key metrics such as water usage, land use, carbon emissions.
- Compare food production methods: Evaluate how various farming techniques (plant based versus animal based) affect environmental sustainability.
- Identify high-impact food products: Determine which foods contribute the most to environmental degradation and assess their sustainability
- Provide data-driven insights: Develop actionable recommendations to reduce the footprint of food production, targeting policy-makers, food producers and consumers.
- Promote sustainable food systems: Suggest strategies to transition toward more sustainable agricultural practices that minimise environmental harm.

Analytic Questions: 
- What is the correlation between land use and carbon emissions for different food products?
- How does eutrophication (nutrient run-off) vary among different types of food production?
- How do plant-based and animal-based foods compare in terms of total carbon emissions per kg of product?
- Which food products have the highest total greenhouse gas emissions per kg of food product?
-  Which food products have the highest eutrophication potential (nutrient runoff) per kg of product?
-  
- What are the main contributors to greenhouse gas emissions in food production and how can they be reduced?
-  What policy interventions (e.g., carbon taxes, incentives for sustainable farming) could help reduce the environmental footprint of food production?


### 2. Data Understanding:

 The dataset contains most 43 most common foods grown across the globe and 23 columns as their respective land, water usage and carbon footprints. Variables include:

a. Land use change - Kg CO2 - equivalents per kg product

b. Animal Feed - Kg CO2 - equivalents per kg product

c. Farm - Kg CO2 - equivalents per kg product

d. Processing - Kg CO2 - equivalents per kg product

e. Transport - Kg CO2 - equivalents per kg product

f. Packaging - Kg CO2 - equivalents per kg product

g. Retail - Kg CO2 - equivalents per kg product

These represent greenhouse gas emissions per kg of food product(Kg CO2 - equivalents per kg product) across different stages in the life-cycle of food production.

### 3. Data Preparation: 

To ensure the data was ready for analysis, a meticulous data preparation process was carried out as follows: 

- Cleaning of column names: The column names were cleaned to ensure standardisation and consistency
- Correction of column names: The column name packging was corrected to packaging.
- Checking data structure: The overall structure of the dataset was examined.
- Duplicate check: No duplicate entries were found.
- Handling Missing Values:

![image](https://github.com/user-attachments/assets/658c46d5-e994-426c-93da-3530661ccb7c) 

The bar chart displays the number of missing values for different variables in a dataset. The x-axis represents the number of missing values while the y-axis lists the variables.

From the chart, the variables related to water use, land use, greenhouse gas emissions and eutrophying emissions per 100g protein or per 1000 kcal have the most missing values, with some having close to 18 missing entries. On the other hand, variables related to food production stages such as transport, retail, processing, packaging, farm and animal feed no missing data.

This suggests that the dataset is more complete for food production stages or processes but has gaps in environmental impact data, especially for nutrient-based metrics.

To maintain data integrity and avoid biased imputations the missing values were dropped from the dataset.
