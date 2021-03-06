# Climate change in the South and Southeast US climate regions

# Research Proposal
The Earth is warming up at an alarming pace mostly due to high increase of carbon dioxide in the atmosphere caused by human activity (burning of fossil-fuels, methane from land-use, deforestation, …). Drastic steps need to be taken to keep the Earth’s average temperature increase below 2-degree Celsius (C), a critical threshold which emerged from the 2015 Paris accord, and thus avoid more extreme and costly events due to climate change, some of which already upon us here in the US (flood and drought, sea level rise, hurricanes, water and food scarcity…). The goal of this study is two-fold:
- First to understand if the South and the Southeast regions in the US have been warming up evenly for the past 125 years as the two climate regions share the same latitudes, diverse topography and proximity to large bodies of water. 
- Second, to investigate if there have been differences in average annual temperatures between the past two decades in the South of the US, which has seen more costly billion-dollar weather disaster events than the rest of the country.  

This study will supplement the wealth of scientific information about global warming to the public and policymakers in those two regions and support the need to take immediate steps to mitigate climate change.


# Data
The Washington’s Post released data (https://github.com/washingtonpost/data-2C-beyond-the-limit-usa/blob/main/data/processed/climdiv_county_year.csv) that compiled annual mean temperatures for counties in the US Lower 48 states, from 1895 to 2019. In this study, I will use those data edited to include state’s name as extra variable, which can be found at this link https://drive.google.com/file/d/19fY-I--dcGFKdwNHaJl4YccMo53NZqmh/view?usp=sharing.


# Research Design
My two hypotheses are that there are no differences in average annual temperatures between the South and Southeast regions from 1895 to 2019, and that in the South there are no differences in mean annual temperatures between the past two decades. If these hypotheses are correct, then we can rest assured that this Southern part of the US is not yet affected by global warming and as long as it stays that way, this region can be on par to stay below the 2-degree C target. These two hypotheses are my null hypotheses.

For this analysis, I create four DataFrames, two for each hypothesis. For the hypothesis including data from the South and Southeast, I use two DataFrames, one containing annual temperatures for each county in each state in the South and the other in the Southeast, from 1895 through 2019. Each DataFrame has temperatures in degrees C and Fahrenheit (F), I will work with degrees Celsius (C). Both datasets were recorded at different locations and are thus independent. For the second hypothesis including uniquely temperature data from the South, I will create two DataFrames, one containing annual temperatures for each county in each state in the decade 2000-2009, and the other for the decade 2010-2019. Each DataFrame has temperatures in degrees C and F, I will work with degrees C. Both datasets were recorded at the same location, but in different decades and are thus dependent.

For each hypothesis, I will look at the distributions of both datasets to investigate if they are close to normality, based on their histogram, skewness and kurtosis. If they are, then I will conduct a t-test for both independent and dependent samples at the two-tail, 95% confidence interval. If they are not, I will perform a Kruskal test. In any case, I will compare the p-value of the hypothesis testing result to my target significance level of 0.05. If p-value is less than 0.05, I will reject the null hypothesis and suggest its alternative. Otherwise, I will fail to reject the null and would not be able to suggest its alternative.


# Audience
This analysis will be valuable for the public and policymakers in the South and Southeast regions of the US. Having measurable metrics in the terms of annual temperatures that highlight how two regions with similar latitudes, diverse topography and proximity to large bodies of water compare, will help understand if both regions are warming up evenly and if not will support the need to take immediate mitigating steps. It will also help grasp if the South is on par to meeting the Paris goals, by looking at the differences in mean annual temperature trends between the first two decades of this century. The findings of this study will reinforce the sense of urgency to act now on taking drastic steps to address climate change and its costly extreme weather events.


