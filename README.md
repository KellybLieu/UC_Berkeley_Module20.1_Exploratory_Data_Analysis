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