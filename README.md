# Predicting water pump functionality in Tanzania using R

## Summary and projects goals
Water is crucial to increase quality of living in rural areas. Using data provided by Tanzania Ministry of Water, I developed a supervised classification model to predict which water pumps need repairs or are totally broken.

Our goal is to address the following questions:
- Which drivers can we rely on to identify faulty water pumps across Tanzania?
- Can we develop a model able to timely detect faulty water pumps?

## Data
Predictive model is trained on data from Taarifa, which aggregates the data from the Tanzania Ministry of Water. You may find and download the data here https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/page/23/ after signing up for the competition. The training data consists of almost 60,000 records of Tanzanian water well pumps across the country and includes features about their location, when they were installed, who installed them, what kind of pump they are, etc., as well as their current functioning status - functional, non-functional, or functional but needs repair.

Out of 59.364 water pumps located across Tanzania, almost 46% are faulty, meaning they need some repairs or are not working at all.

## Model development and results
After collecting the data, we performed some data cleansing activity in R aimed at improving quality of input data. Then we applied a Random Forest algorithm in R that is 98% accurate in detecting which water pumps are at greater risk of not functioning properly. After developing the model, we also estimate variable importance in order to understand which factors are more influential.
