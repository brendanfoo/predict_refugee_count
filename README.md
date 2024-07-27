# Understanding and Predicting Internal Displacement from Global Floods

# Abstract

Our research aims to address critical gaps in current predictive modeling methods for flood-induced displacements amid escalating global climate change. Using a unified dataset from various sources, including the UN Global Internal Displacement Database, our study employs different robust machine learning models such as random forests for classification and support vector machine for regression. Challenges of scattered and unstandardized data are noted, limiting our analysis to ~60% of the countries. Our findings emphasize the need for improved data quality and standardization for more reliable predictive modeling of flood-induced displacement.

# Problem & Motivation
Climate change is one of the biggest threats facing humanity today. According to the Intergovernmental Panel on Climate Change, approximately 3.5 billion people were living in countries with a high vulnerability to climate change in 2022, and 31.8 million people were internally displaced within the borders of their country due to weather-related hazards. Of the 31.8 million displacements, 60% were due to floods. Flood-caused internal displacements are a rather new area with little existing research and data, and no predictive technologies currently exist to identify or protect those impacted by climate change. Motivated by the lack of research in this field, our project aims to predict the relative level of internally displaced individuals in a specific region of the world if a flood were to occur. We believe that such a model would be highly beneficial in terms of serving as an early warning sign for at-risk populations and also as a guide for resource allocation for humanitarian aid groups. 

# Data Source & Data Science Approach
Our project’s data combines four datasets (GIDD, ND-GAIN, Flood Archive, Census) into one that encodes, for each flood event, the time and place, magnitude, causes, and features of the country such as population measures and various factors related to preparedness for natural disasters. GIDD refers to the UN Global Internal Displacement Database, which is the base set of flood events. ND-GAIN refers to the Notre Dame Global Adaptation Initiative, and it supplements the GIDD dataset with descriptions of how well each country is prepared for flood events based on factors including infrastructure, economy, and more. Flood Archive is from the University of Colorado and includes information such as the magnitude of each flood event—data that was found manually by professors at the university through news reports and articles. Lastly, U.S. Census Bureau data provides population counts and population density for each country.
After combining these datasets, we performed exploratory data analysis and model selection. Our final main models included (1) random forest classification, which predicted categorical outcomes and was useful for understanding the space and trends, and (2) support vector machine regression, which predicted continuous outcomes and was useful for hard predictions on numbers. 

# Evaluation
The performance of our models is evaluated based on recall, precision, accuracy, and root mean square error. For the random forest classification, the model’s top features were also identified and a confusion matrix showed the model’s performance for each class. For the support vector machine regression, we evaluated our model’s performance using the root mean square error.

# Key Learnings & Impact
Throughout our project, it became increasingly clear that there are currently barriers to the data collection process and data gaps in the existing data. Based on our research, access to relevant data for internal displacement due to flooding is very limited and dispersed. Moreover, there are varying definitions of what counts as a distinct flood event to different data sources. These limitations led us to conclude that this field of study is incredibly overlooked and could benefit from more attention, particularly in the data collection process.
For now, we have a few proposed solutions to address these limitations. First, having a publicly available and centralized database would help bring all the scattered data together. Next, having standardized definitions of climate events would help minimize confusion around the topic. Lastly, the adoption of a standard for assessing the impacts of climate change on flood displacement risk would greatly improve the data analysis in this field.
