# Overview
Food production is one of the most significant contributors to environmental degradation, including issues such as climate change, water scarcity and biodiversity loss. The agricultural sector's environmental footprint varies widely across different food products, farming methods and geographical locations. Understanding the environmental impacts of food production is essential for developing more sustainable practices, reducing ecological footprints and making informed policy and consumer choices. 

This project focuses on analysing the environmental impact of food production, emphasising key metrics such as carbon emissions, water usage, land use and biodiversity loss. This analysis aims to uncover patterns and provide actionable recommendations for more sustainable food systems, by leveraging data on food production and environmental factors

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


#### Data visualisation of the top ten total emissions (Kg CO2) by food products

![image](https://github.com/user-attachments/assets/d499da2c-4c92-40a1-9ad1-beffc2c19e5a)

The bar chart depicts the distribution of the top ten total emissions by food products. The y-axis shows total emissions whilst the x-axis lists different food products. Each food product is represented by a unique colour in the legend on the right.

From the chart, Beef (beef herd) demonstrates the highest emissions by a considerable margin followed by Beef (dairy herd) which also has significant emissions but substantially lower in comparison. The remaining food products have relatively minor emissions compared to beef. This indicates that beef production has a significantly higher environmental impact regarding emissions compared to other food products.

According to the World Wildlife Fund (2025), Beef production has a higher environmental impact than other food sources due to factors like land use for grazing and crop production, greenhouse gas emissions from cattle and water pollution from waste run-off as well as deforestation from cattle ranching.

As stated by the Beef Research Council, beef production requires vast amounts of land both for grazing cattle and for growing feed crops. Globally, a significant portion of agricultural land is used for livestock including cattle and a large area of rainforests is destroyed to create grazing land.

Cattle are a major source of greenhouse gas emissions particularly methane which is a potent greenhouse gas. Methane is released during the digestive process of cattle and also from manure management. The production of feed crops for cattle also contributes to greenhouse gas emissions (Beef Research Council, 2025).

Cattle waste, if not properly managed, can pollute water sources with nitrates, phosphorus and pathogens. Water used for livestock production can also be a significant burden on water resources especially in arid regions (Beef Research Council, 2025). The Food and Agriculture Organisation has written, "The livestock sector is growing and intensifying faster than crop production in almost all countries. The associated waste including manure has serious implications for water quality (Rosie's Farm Sanctuary, 2025).

Cattle ranching is a major driver of deforestation especially in regions like the Amazon rainforest where land is cleared to create grazing pastures. Deforestation contributes to climate change, biodiversity loss and soil degradation (Rosie's Farm Sanctuary, 2025).


#### Data visualisation of plant-based and animal-based on land use (m² per 100g protein) versus greenhouse gas emissions (kg CO2-eq per 100g protein)

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


#### Box plot to detect outliers in Greenhouse Gas Emissions (kg CO₂-eq per 100g protein)

![image](https://github.com/user-attachments/assets/e7c25b8d-f17a-4e3f-bf7f-be323bb1fad1)

The box plot compares greenhouse gas emissions by category. The box is for animal and plant-based foods that are quite similar. Both categories have high emission outliers, but the most extreme values is in the plant-based category (one point above 70 kg CO₂-eq). There's also an outlier in the animal-based category at 50 kg CO₂-eq.


#### Box plot to detect outliers in Land Use (m² per 100g protein) 

![image](https://github.com/user-attachments/assets/2ec361f2-dc85-4ec1-999f-b776a8f67cbd)

The box plot compares land use by food category. Animal-based food has a higher median land use than plant-based food. The IQR is wider for animal-based food, indicating greater variability. 

Both categories have extremely high land use outliers. The highest land use (above 150m2 per 100g protein) is likely a type of livestock, likely to be lamb.

Some plant-based food also have a high land use, possibly dark chocolate.


#### Investigating the Outliers Further 

![image](https://github.com/user-attachments/assets/9a257097-ddfc-4237-bdfc-a16d53f2748b) 

#### Outliers in Greenhouse Gas Emissions (kg CO₂-eq per 100g protein)

Dark Chocolate has the highest emissions, even more than beef. Which is likely due to deforestation (for cocoa plantations), transport emissions and processing.

Beef (beef herd) is known for methane emissions from cattle digestion. Coffee is possibly due to deforestation, water use and energy-intensive processing. 

Coffee production has a significant environmental impact, including deforestation, water pollution and carbon emissions, but sustainable practices like shade-grown coffee and organic farming can mitigate these issues (Green Coffee Bean, 2025).

From a climate point of view, deforestation is catastrophic. Burning timber releases CO2, but beyond that, it also frees carbon stored in the soil and limits the forest's ability to absorb carbon in the future. This explains why deforestation accounts for roughly 95% of the greenhouse gas emissions linked to cocoa beans. At the same time, it also poses a major threat to biodiversity (Le Monde, 2025).

Next, emissions from chocolate processing need to be taken into account – especially for highly processed products such as chocolate-covered biscuits or chocolate spreads. And finally, there is transport, though its impact is relatively minor in comparison (Le Monde, 2025).

![image](https://github.com/user-attachments/assets/1384d580-6d5a-4876-a31f-77cbe44660d8) 

#### Outliers in Land Use (m² per 100g protein)

Lamb & Mutton require even more land than beef.  Beef (beef herd) is high due to the large land area needed for grazing and feed production. Dark Chocolate again appears as a high-impact product, reflecting the land-intensive nature of cocoa farming.



#### Exploratory Data Analysis On Water Use (Freshwater Withdrawals & Scarcity-Weighted Water Use) 

#### Data Visualisation on top freshwater consuming food products litres per 1000kcal

![image](https://github.com/user-attachments/assets/1a94aa27-2668-4e30-bd2a-5db1725cf107) 

The bar chart depicts the distribution of the top ten water-consuming food products. Farmed fish is the highest water consumer, followed by Tomatoes and Cheese. Rice and Nuts are also water consumers. 

Cheese, Milk, Beef (dairy herd), Pig, Milk and Farmed Fish are the most water-intensive animal-based food products in this ranking. 

While all food production requires water, plant-based foods generally require significantly less water than animal products, making them a more water-efficient choice (Colorado Sun, 2022). Animal agriculture consumes high amounts of water and pollutes freshwater ecosystems (Livvie, 2025) also, raising livestock, especially beef, requires vast amounts of water for feed production, drinking water, and cleaning (Livvie, 2025).

From the chart, tomatoes are the most water-consuming plant-based food product, which is supported by EOS (2025), stating that tomato cultivation can be water-intensive, with some studies suggesting that producing 1 kg of tomatoes can require anywhere from 4 to 300 liters of water, depending on the growing method and efficiency.


#### Box plot on plant-based versus animal-based freshwater use litres per 1000kcal

![image](https://github.com/user-attachments/assets/2730de17-d78c-4b46-82d4-c5c7587b932e)


The box plot compares freshwater use by food category. Animal-based food has a higher median land use than plant-based food per 1000kcal. Plant-based food exhibit a wider range, with some food product requiring very little water, while others require more. Outliers in both categories suggest extreme water consumption for specific food products.


#### Investigating the Outliers Further in Freshwater Withdrawals (litres per 1000 kcal)

![Image](https://github.com/user-attachments/assets/9aa957e3-b2c6-4ffc-92df-00648ba81373)

This visualisation highlights the outliers in freshwater withdrawals (litres per 1000 kcal). Fish (farmed) is the highest outlier among animal-based food product. Tomatoes is the highest outlier among plant-based food product. Both require significantly more water than the median food product.


#### Box plot on plant-based versus animal-based scarcity- weighted use litres per 1000kcal

![Image](https://github.com/user-attachments/assets/fe006d95-76ee-4765-b437-2f912d6d4a2f) 

This box plot compares scarcity-weighted water use (litres per 1000 kcal) for animal-based and plant-based food categories.

Animal-based food have a higher median and spread of scarcity-weighted water use than plant-based food.The variation within plant-based food shows relatively low water use while others have values close to animal-based food.

The scarcity-weighted water use box-plot doesn't show distinct outliers. The distribution suggests that both animal-based and plant-based food have a wide range, but no extreme points that fall significantly outside the whiskers.



#### Scatter Plot: Freshwater Withdrawals (litres per 1000kcal) versus Scarcity-Weighted Water Use (litres per 1000kcal)

![image](https://github.com/user-attachments/assets/b8b48290-4dcc-4e27-a69d-b83f3fab5d70)

The scatter plot shows a distribution of freshwater withdrawals versus scarcity weighted water use. 

Freshwater withdrawals (litres per 1000kcal) measures the total amount of water taken from sources, while scarcity-weighted water use (litres per 1000kcal) considers the water's availability and stress levels in the region where it's used. 

Both plant-based and animal-based foods show variation in how their water use translates into environmental stress.


# Recommendations & Conclusion

## Strategies for land use & greenhouse emission of beef food product

Global Food Institute (2025), states that using alternative proteins helps reduce air and water pollution significantly. With the use of plants, fermentation and cell cultivation instead of livestock, the production of alternative proteins does not emit the toxic air pollutants including ammonia, hydrogen sulfide and particulate matter as conventional meat production. Also ,there will be no discharge of animal waste. The discharge of nitrogen and phosphorus which stimulates the growth of algal blooms that impair water  quality is reduced by using alternative proteins.

Moving towards alternative proteins will promote clean water and air as well as improving ecosystems and the health of communities as it also meets increasing protein demand. 

Policy-makers should invest in alternative proteins for a secure, sustainable food supply. The support of alternative protein innovation and commercialisation, will increase food security (Global Food Institute, 2025).


### Alternative Proteins

Science Direct (2025) states that alternative proteins are healthier, more sustainable and environmentally friendly. Alternative proteins are food products, often meat substitutes, derived from sources other than traditional animal-based proteins, like plant-based proteins, cultured meat or fermented products, aiming to be healthier and more sustainable. 

Alternative Proteins are gaining popularity due to concerns about the environmental impact of traditional meat production, as well as growing interest in plant-based diets and healthier eating habits (Liu, 2018).

### Types of Alternative Proteins: 

Plant-based Proteins: These are derived from plants and include plants like legumes, soy, nuts and seeds, grains, mycoprotein (derived from fungi for its meat-like texture) (Finnigan, 2011)

Cultured Meat: Also known as lab-grown meat, this meat is produced from animal cells in a lab, rather than slaughtering animals (Learn About Ag, n.d.).

Fermented Proteins: These are proteins produced through fermentation such as mycoprotein or certain plant-based proteins (FoodNavigator, 2024).

Algae and Insects: There are are emerging as potential sources of alternative protein (Lui, 2018).


### Benefits of Alternative Proteins:

Sustainability: Alternative Proteins often require less land, water and resources to produce compared to traditional meat production (Lui, 2018).

Health: Many plant-based proteins are lower in saturated fat and cholesterol than animal-based proteins and can be a good source of fiber and other nutrients (Science Direct, 2025).

Ethical considerations: For those who choose to avoid animal products, alternative proteins offer a way to meet their protein needs without consuming animal products (Science Direct, 2025).


## Strategies for reducing environmental impact of coffee

Implementing sustainable agricultural methods represents a crucial approach to minimizing the environmental impact of coffee production. One notable example is shade-grown cultivation, where coffee plants are grown beneath a forest canopy. This technique serves the dual purpose of preventing deforestation while fostering biodiversity and ecological health. The trees provide a natural habitat for a wide variety of species, helping preserve biodiversity. Additionally, they assist in preventing soil erosion and maintaining soil health, which can otherwise be severely compromised due to excessive coffee farming (Green Bean Coffee, 2025)

Another sustainable practice is organic coffee bean farming, that can drastically reduce coffee's environmental impact. Organic methods avoid the use of synthetic fertilisers and pesticides, unlike traditional coffee farming. According to Green Bean Coffee (2025), these chemicals pose a threat to aquatic life and contaminate water bodies. Organic farming not only protect the ecological balance of the various areas coffee is grown in but also helps to preserves our water sources.


# References 
- Beef Research Council. (n.d.). Environmental footprint of beef production. Retrieved from https://www.beefresearch.ca/topics/environmental-footprint-of-beef-production/#:~:text=The%20beef%20environmental%20footprint%20has,produced%20by%20plants%20and%20animals.
- World Wildlife Fund. (2025). Beef production and its environmental impact. Retrieved from https://www.worldwildlife.org/industries/beef#:~:text=Beef%20production%20has%20a%20considerable,emissions%20from%20human%2Drelated%20activities.
- Rosie's Farm Sanctuary. (2025). Environmental impact of beef production. Retrieved from https://rosiesfarmsanctuary.org/learn/environment/#:~:text=Beef%20production%20alone%20contributes%2041%%20of%20all,by%20an%20ever%2Drising%20international%20demand%20for%20beef.
- Global Food Institute. (2025). Environmental impacts of alternative proteins. Retrieved from https://gfi.org/resource/environmental-impacts-of-alternative-proteins/
- Green Bean Coffee. (2025). Sustainability and the environmental impacts of coffee. Retrieved from https://www.greenbeancoffee.com.au/blogs/news/sustainability-and-the-environmental-impacts-of-coffee#:~:text=Organic%20coffee%20cultivation%20offers%20numerous,depends%20on%20your%20individual%20tastes.
- Le Monde. (2025). What is chocolate's carbon footprint? Retrieved from https://www.lemonde.fr/en/environment/article/2025/02/14/what-is-chocolate-s-carbon-footprint_6738165_114.html#:~:text=Three%20key%20stages%20drive%20the,chemical%20inputs%2C%20deplete%20soil%20quality.
- Colorado Sun. (2022). Water, drought and the environmental impact of agriculture: The food we produce matters. Retrieved from https://coloradosun.com/2022/09/07/water-drought-agriculture-food-production-meat-plants-opinion/#:~:text=While%20any%20plant%2Dbased%20food,only%20uses%20about%20one%20gallon.
- Livvie. (2025). Save water with a vegetarian or vegan diet. Retrieved from https://www.livvie.co/save-water-with-a-vegetarian-or-vegan-diet/#:~:text=How%20Vegetarian%20and%20Vegan%20Diets,for%20more%20information%20and%20sources.
- EOS. (2025). How to grow tomatoes. Retrieved from https://eos.com/blog/how-to-grow-tomatoes/#:~:text=Water,them%20less%20susceptible%20to%20drought.
- Our World in Data. (2025). Eutrophying emissions per protein. Retrieved from https://ourworldindata.org/grapher/eutrophying-emissions-protein.
- Our World in Data. (2025). Water use and stress in global food production. Retrieved from https://ourworldindata.org/water-use-stress#:~:text=Water%20use%20of%20food%20products%20Globally%2C%2070,1000%20kilocalories%2C%20and%20100%20grams%20of%20protein.
- ScienceDirect. (2025). Alternate proteins (APs): Healthier, sustainable, and climate-friendly food alternatives. Retrieved from https://www.sciencedirect.com/science/article/pii/S096399692301027X#:~:text=Alternate%20proteins%20(APs)%20are%20healthier,bioavailability%2C%20nutritional%20equivalency%20and%20digestibility.
- Liu, W. (2018). Fact Sheet: Alternative Protein. University of Nottingham. Retrieved from https://www.nottingham.ac.uk/biosciences/documents/business/food-innovation-centre/food-waste-alternative-protein-event-2018/fact-sheet-alternative-protein-dr-wentao-liu.pdf.
- Finnigan, T. (2011). The nutritional properties of mycoprotein are essential for meat alternative development. ScienceDirect. Retrieved from https://www.sciencedirect.com/science/article/abs/pii/S0308814624031868#:~:text=The%20nutritional%20properties%20of%20mycoprotein%20are%20essential,the%20structure%20of%20meat%20myofibers%20(Finnigan%2C%202011).
- Learn About Ag. (n.d.). Alternative protein sources. Retrieved from https://learnaboutag.org/matrix/lesson/print/709/
- FoodNavigator. (2024, January 17). Diversified protein sourcing and the path to mainstream adoption. Retrieved from https://www.foodnavigator.com/Article/2024/01/17/diversified-protein-sourcing-and-the-path-to-mainstream-adoption/#:~:text=Alternative%20sources%20of%20protein%20emerging,as%20animal%20and%20plant%20proteins.



