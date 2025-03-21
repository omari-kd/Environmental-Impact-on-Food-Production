# Overview
Food production is one of the most significant contributors to environmental degradation, including issues such as climate change, water scarcity and biodiversity loss. The agricultural sector's environmental footprint varies widely across different food products, farming methods and geographical locations. Understanding the environmental impacts of food production is essential for developing more sustainable practices, reducing ecological footprints and making informed policy and consumer choices. 

This project focuses on analysing the environmental impact of food production, with an emphasis on key metrics such as carbon emissions, water usage, land use and biodiversity loss. By leveraging data on food production and environmental factors, this analysis aims to uncover patterns and provide actionable recommendations for more sustainable food systems. 

The goal of this project is to assess the environmental impact of food production at both macro and micro levels and propose data-driven insights to mitigate the negative effects of food production on the environment. This will help policymakers, environmentalists, food producers and consumers make more informed decisions that support sustainability.

## Crisp DM Framework 

The analysis followed the CRISP-DM methodology, which includes the following stages:

Business Understanding

a. Define the project objectives and business goals

b. Identify key questions that need to be answered

Data Understanding 

a. Collect data from various sources

b. Explore the data (e.g., summary statistics, missing values, patterns)

c. Identify potential issues like inconsistencies, duplicates and outliers

Data Preparation

a. Clean and preprocess the data

b. Handle missing values and inconsistencies

c. Transform data into the right format for analysis


Analysis and Visualisation

a. Exploratory Data Analysis

b. Confirmatory Data Analysis

Recommendations

### 1. Business Understanding

The objectives were defined below, followed by the formulation of analytic questions to guide the analysis.

Objectives 
- Assess the environmental impact of food production: Analyse the environmental impact of these different food products based on key metrics such as water usage, land use, carbon emissions
- Compare food production methods: Evaluate how various farming techniques (plant based versus animal based) affect environmental sustainability
- Identify high-impact food products: Determine which foods contribute the most to environmental degradation and assess their sustainability
- Provide data-driven insights: Develop actionable recommendations to reduce the footprint of food production, targeting policy-makers, food producers and consumers
- Promote sustainable food systems: Suggest strategies to transition toward more sustainable agricultural practices that minimise environmental harm

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
- Correction of column names: The column name packging was corrected to packaging
- Checking data structure: The overall structure of the dataset was examined
- Duplicate check: No duplicate entries were found
- Handling Missing Values:

![image](https://github.com/user-attachments/assets/658c46d5-e994-426c-93da-3530661ccb7c) 

The bar chart displays the missing values for different variables in a dataset. The x-axis represents the  missing values while the y-axis lists the variables.

From the chart, the variables related to water use, land use, greenhouse gas emissions and eutrophying emissions per 100g protein or 1000 kcal have the most missing values, with some having close to 18 missing entries. On the other hand, variables related to food production stages such as transport, retail, processing, packaging, farm and animal feed no missing data.

This suggests that the dataset is more complete for food production stages or processes but has gaps in environmental impact data, especially for nutrient-based metrics.

To maintain data integrity and avoid biased imputations the missing values were dropped from the dataset.

### Analysis and Visualisation

#### Exploratory Data Analysis 


#### Data visualisation of the top ten total emissions by food products 

![image](https://github.com/user-attachments/assets/d499da2c-4c92-40a1-9ad1-beffc2c19e5a)

The bar chart depicts the distribution of the top ten total emissions by food products. The y-axis shows total emissions whilst the x-axis lists different food products. Each food product is represented by a unique colour in the legend on the right.

From the chart, Beef (beef herd) demonstrates the highest emissions by a considerable margin followed by Beef (dairy herd) which also has significant emissions but substantially lower in comparison. The remaining food products have relatively minor emissions compared to beef. Cane Sugar and Beet Sugar have slightly elevated emissions than most other products apart from beef but remain much lower overall.

This indicates that beef production has a significantly higher environmental impact regarding emissions compared to other food products.

According to the World Wildlife Fund (2025), Beef production has a higher environmental impact than other food sources due to factors like land use for grazing and crop production, greenhouse gas emissions from cattle and water pollution from waste run-off as well as deforestation from cattle ranching.

As stated by the Beef Research Council, beef production requires vast amounts of land both for grazing cattle and for growing feed crops. Globally, a significant portion of agricultural land is used for livestock including cattle and a large area of rainforests is destroyed to create grazing land.

Cattle are a major source of greenhouse gas emissions particularly methane which is a potent greenhouse gas. Methane is released during the digestive process of cattle and also from manure management. The production of feed crops for cattle also contributes to greenhouse gas emissions (Beef Research Council, 2025).

Cattle waste, if not properly managed, can pollute water sources with nitrates, phosphorus and pathogens. Water used for livestock production can also be a significant burden on water resources especially in arid regions (Beef Research Council, 2025). The Food and Agriculture Organisation has written, "The livestock sector is growing and intensifying faster than crop production in almost all countries. The associated waste including manure has serious implications for water quality (Rosie's Farm Sanctuary, 2025).

Cattle ranching is a major driver of deforestation especially in regions like the Amazon rainforest where land is cleared to create grazing pastures. Deforestation contributes to climate change, biodiversity loss and soil degradation (Rosie's Farm Sanctuary, 2025).


#### Data visualisation of plant-based and animal based on land use versus greenhouse gas emissions

![image](https://github.com/user-attachments/assets/13ee8e1d-e8f7-4d2b-adce-13de8b59d545) 

This scatter plot shows the relationship between land use(x-axis) and greenhouse gas emissions (y-axis) for different food categories, split into animal-based (red points & dashed red trend line) and plant-based foods (blue points & dashed blue trend line). 

The animal-based foods generally do have lower land use. The trend line is relatively flat, suggesting that increasing land use does not significantly increase emissions within this category.

The plant-based foods show a wider range of land use, with one food product using significantly more land. The trend line is much steeper, indicating that higher land use is strongly associated with higher emission in this category.

This data has more plant-based products than animal-based products, but the goal to reduce greenhouse gas emissions, shift from animal-based to plant-based proteins might be beneficial. However, for land conservation, certain plant-based foods could still have a significant impact, depending on the type.

Global Food Institute stated that, by using plants, fermentation or cell cultivation instead of livestock, the production of alternative proteins does not emit the same toxic air pollutants that is, ammonia, particulate matter and hydrogen sulfide; as conventional meat production. Similarly, because there is no animal waste to discharge and fewer crops and fertilisers are needed, alternative proteins reduce the discharge of nitrogen and phosphorus, which stimulate the growth of algal blooms that impair water quality. A shift toward alternative proteins can keep our air and water clean, improving the health of communities and ecosystems while meeting increasing protein demand.


#### Summary of greenhouse gas emission (kg CO₂-eq per 100g protein) 

The minimum greenhouse gas emission is 0.26, which is very low in CO2 emissions.

1St Quartile: 25% of the food product emission is below 4.28 kg CO₂-eq.

Median: Half of the food products have emissions is 7.05 kg CO₂-eq.

Skewness: The Mean is higher than the median, suggesting a right-skewed distribution (some foods have extremely high emissions)

3Rd Quartile:  75% of the foods have emissions of about 15.69 kg CO₂-eq.

Maximum: The highest emission food products produces 93.3 kg CO₂-eq  which is far above the mean, confirming outliers.

Most foods have emissions below 16 kg CO₂-eq, but a few high-impact foods (an example is beef) push the mean much higher.


#### Summary Land Use (m² per 100g protein) 

The minimum land use is just 3 m² per 100g protein. 

1St Quartile: 25% of the food product requires 5.132 m².

Median: Half of the food product needs 9.33 m².

Mean: Again, much higher than the median, indicating a some food products take up a lot of land.

3Rd Quartile: 75% of foods require 24.83 m² 

Maximum: Food products require almost 185 m² per 100g protein which is massively higher than the rest (likely beef).


#### Box plot to detect outliers in Greenhouse Gas Emissions 

![image](https://github.com/user-attachments/assets/e7c25b8d-f17a-4e3f-bf7f-be323bb1fad1)

The box plot compares greenhouse gas emissions by category. The box is for animal and plant-based foods that are quite similar. Both categories have high emission outliers, but the most extreme values is in the plant-based category (one point above 70 kg CO₂-eq). There's also an outlier in the animal-based category at 50 kg CO₂-eq.


#### Box plot to detect outliers in Land Use  

![image](https://github.com/user-attachments/assets/2ec361f2-dc85-4ec1-999f-b776a8f67cbd)

The box plot compares land use by food category. Animal-based food has a higher median land use than plant-based food. The IQR is wider for animal-based food, indicating greater variability. 

Both categories have extremely high land use outliers. The highest land use (above 150m2 per 100g protein) is likely a type of livestock, likely to be lamb.

Some plant-based food also have a high land use, possibly dark chocolate.



# Recommendations & Conclusion


# References 
- Beef Research Council. (n.d.). Environmental footprint of beef production. Retrieved from https://www.beefresearch.ca/topics/environmental-footprint-of-beef-production/#:~:text=The%20beef%20environmental%20footprint%20has,produced%20by%20plants%20and%20animals.
- World Wildlife Fund. (2025). Beef production and its environmental impact. Retrieved from https://www.worldwildlife.org/industries/beef#:~:text=Beef%20production%20has%20a%20considerable,emissions%20from%20human%2Drelated%20activities.
- Rosie's Farm Sanctuary. (2025). Environmental impact of beef production. Retrieved from https://rosiesfarmsanctuary.org/learn/environment/#:~:text=Beef%20production%20alone%20contributes%2041%%20of%20all,by%20an%20ever%2Drising%20international%20demand%20for%20beef.
- Global Food Institute. (2025). Environmental impacts of alternative proteins. Retrieved from https://gfi.org/resource/environmental-impacts-of-alternative-proteins/

