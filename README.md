# UC_Berkeley_Module20.1_Exploratory_Data_Analysis
Author: Kelly Lieu <br/>

BACKGROUND <br/>
My goal is for this capstone is to learn and practice how to apply AI/ML principles with storytelling data visualization techniques. It was important to me to choose a dataset that was easy to obtain and a topic that I can learn from to apply at home or at work. The data comes from Kaggle called, "Longevity Factors." 

WE WILL EXPLORE <br/>
Which features provide most gain in years of life?
Which factors provide the most gain in years of life for females?
What are the top features based on the weighted impact of strength of science on years?
How do the stronger science features rank against the suggestive features?
What other insights can I derive from the data?

INITIAL EAD FINDINGS REPORT <br/>
In the exploratory data analysis, I began by importing the necessary libraries and loading the dataset for an initial preview. I checked for missing values and visualized them using a heatmap, which revealed that the comments column contained the most nulls. Consequently, I removed irrelevant columns such as comment, note, sources, links, and id. I then focused on the numerical features, using histograms to examine the distribution of values. The analysis showed that the majority of years gained or lost ranged between 2 and 6 years, with a few extreme negative outliers (e.g., -25 and -10 years). Most contributing factors were associated with a low level of scientific strength. I used boxplots to further identify outliers, but the science column offered little insight due to its limited range of values (1, 2, and 3). Lastly, the pairplot did not reveal any meaningful correlations, as there were only two numerical features available.

SECONDARY EAD FINDINGS REPORT <br/>
Since the Initial EAD was inconclusive, I proceeded with further investigating whether the factors impacting lifestyle were impacted by strength of science and furthermore comparing the factors between genders. First, I computed the weighted impact of each factor by multiplying years gained/lost feature with strength of science as a number (1, 2, or 3). Immediately, it provided a better sense of magnitude and importance of each factor, with science-driven as a better indicator that the factor was more reliable although knowing that the actual years gained/lost in life is no longer accurate. 

Despite loss of accuracy, I visualized the top 10 science-backed longevity factors in a barplot, as shown in the Jupyter notebook. To name a few, the top 3 are: 1) Lifestyle of non-smoking, exercising, and healthy eating; 2) Healthy Eating; 3) Good marriage; 4) Good genetics; 5) More money; 6) Avoid cancer...

I then continue my analysis to compare the factors that were relevant to women. To do so, I had to cleanse the data and replace some values to normalize the data so I can properly identify the factors that pertain to only women or men. In doing so, I created another barplot with this data to compare the top 10 factors for women against the previous factors that included factors that only pertained to men. To list a few, the top 10 science-backed factors affecting longevity for women are: 1) Lifestyle of non-smoking, exercising, and healthy eating; 2) Healthy Eating; 3) Good marriage

There is overlap in most of the longevity factors between both genders. The key difference is for a men, spending time with women was ranked #7 (a male-specific factor), whereas women did not have that factor. As a trade-off the barplot for women had "Pets - dogs" ranked at #10, where it was #13 in the barplot for both genders.

For the top contributors of reduced longevity are shared between both plots, indicating universal risks that are science-based regardless of gender. To name a few: 1) Mental illness; 2) Smoking; 3) Obesity; 4) Alcohol (heavy abuse). The top 4 seem to have the heaviest impact, whereas the subsequent 4 seem insignificant. 

Furthermore, I will add that I attempted to feature engineer my dataset, however this dataset is very small and it was not necessary to use one-hot encoding nor polynomial features. It was insightful and I plan on 

FEATURE ENGINEERING
The next sequence of steps is to perform feature engineering to prepare my dataset for building a model. Below I will start with a copy of the previous dataframe and perform the following:<br/>

Identify categorical variables
Use one-hot encoder on categorical features
Create interaction terms (multiply factor and strength of science)
Create polynomial features and create a dataframe (except target col)
Create combined original dataframe with polynomial dataframe
Use StandardScaler to scale all my features (except target col)
Add back target column and I am ready to build my model


TECHNIQUES FOR CAPSTONE <br/>
Exploratory Data Analysis (EAD) and Visualize Results
Feature Engineering
Fit and Train Multiple Models
Compare Models Using GridSearchCV
Choose the Best Model
Perform Hyperparameter Tuning
Choose the Best Features
Visualize Results of Predictive Analysis


PERSONAL SUCCESS MEASURES <br/>
	1. Did I use data that I was interested in?
	2. Did my model answer my questions to help me further understanding of the topic?
	3. Did I further my understanding of data science techniques, cleansing data, filtering data, calculating data, plotting data?
	4. Did I further my understanding of storytelling with data visualization techniques, using maplotlib style fivethirtyeight?

DATA SOURCE AND CITATION <br/>
• Arvidsson, Joakim. Longevity Factors (2023): URL: https://www.kaggle.com/datasets/joebeachcapital/life-longevity-factors