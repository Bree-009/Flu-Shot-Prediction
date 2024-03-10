![banner](https://github.com/Bree-009/Predicting-Flu-Shot-Vaccine-Uptake/blob/main/flushot%20banner.jpg)

# Predicting Flu-Shot Vaccine Uptake

## Introduction

In 2009, the World Health Organization (W.H.O) declared the H1N1 flu to be a pandemic. That year, the virus caused an estimated 284,400 deaths worldwide. The pandemic was declared over but the H1N1 flu strain became one of the strains that cause seasonal flu. 

Seasonal flu (influenza) is an acute respiratory infection caused by influenza viruses which circulate in all parts of the world. Seasonal influenza is characterized by a sudden onset of fever, cough, headache, muscle and joint pain, severe malaise, sore throat and a runny nose. 
In temperate climates, seasonal epidemics occur mainly during winter, while in tropical regions, influenza may occur throughout the year, causing outbreaks more irregularly; [World Health Organization](https://www.who.int/health-topics/influenza-seasonal#tab=tab_1).


Most people with the flu get better on their own. But flu and its complications can be deadly, especially for people at high risk like the very young, the elderly, pregnant women, health workers and those with serious medical conditions. The seasonal flu vaccine can now help protect against the H1N1 flu and other seasonal flu viruses; [Mayo Clinic](https://www.mayoclinic.org/diseases-conditions/swine-flu/symptoms-causes/syc-20378103#:~:text=Overview,infect%20pigs%2C%20birds%20and%20humans.).


## Problem Statement

**What is the prevailing circumstance?**

Immunization is a global health and development success story, saving millions of lives every year. Vaccines reduce risks of getting a disease by working with the body’s natural defences to build protection; [W.H.O](https://www.who.int/health-topics/vaccines-and-immunization#tab=tab_1). 


**What problem are we trying to solve?**

Despite the benefits of vaccines, many people are still reluctant to get vaccines or vaccinate their children. According to the [National Center for BioTechnology Information](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4869767/#:~:text=Some%20parents%20believe%20that%20the,the%20benefits%20of%20the%20vaccines.), the reasons for vaccine hesitancy can be divided into 4 categories: religious reasons, personal beliefs or philosophical reasons, safety concerns, and a desire for more information from healthcare providers. 


**How the project aims to solve the problem?**

This project aims to develop a predictive model capable of forecasting vaccine uptake by analyzing an individual's background information and behavioral patterns.
Understanding the reasons behind vaccine hesitancy will better enable healthcare personnel to provide the education and awareness that individuals need to make responsible immunization choices.

## Main Objective
The main objective of this project is to develop a predictive model capable of forecasting seasonal flu vaccine uptake by analyzing an individual's background information and behavioral patterns.

## Notebook Structure
1. Business Understanding
2. Reading and understanding the data
3. Data Cleaning
4. Exploratory data analysis
5. Data preprocessing 
6. Modelling 
7. Evaluation 
8. Pickling
9. Limitations and Next Steps
10. Recommendations

## Data Understanding
The data used in this project was obtained from: [DRIVENDATA](https://www.drivendata.org/competitions/66/flu-shot-learning/data/).

The dataset is divided into: training set features and training set labels.

Each row in the dataset represents one person who responded to the National 2009 H1N1 Flu Survey.

The **training set features** contains: *26707 rows* and *35 columns*

The **training set labels** contains: *26707 rows* and *2 columns*

## Data Preparation
This step involved cleaning the data, handling missing values and handling duplicates. 
It ensured that the data wass accurate, complete, and formatted correctly for use in analysis and modelling. 

Exploratory Data Analysis wascperformed  to understand the relationships between variables, identify patterns and gain insights into the dataset. 
This helped in understanding the distribution of the data, which guided model selection and hyperparameter tuning.

Data preprocessing was also performed to transform data into a format that is more suitable for modeling. 
The steps that were undertaken in this step included: Feature Encoding, Feature Selection, Feature Scaling and Data Splitting.

## Modelling
Several models were built and trained using the training dataset. Hyperparameters were tuned to optimize performance.
The performance of the models was evaulated using cross-validation, accuracy, precision and recall.

## Evaluation
As per the metrics,the  **Random Forest after Hyperparameter Tuning Model** performed the best on both training and testing data and had consistent performance in cross-validation. 

The Random forest after Hyperparameter Tuning model was selected over logistic regression after after RFECV because it can capture complex nonlinear relationships between the features and the outcome.

The scores of the Baseline Model were improved from a training accuracy of 74.39% and a testing accuracy of 74.36% , to a training accuracy of 79.75% and a testing accuracy of 77.17%. The F1 Score was improved from 72.20% in training and 71.73% in testing to 77.50% in training and 74.74% in testing. The success metric of 75% was achieved in accuracy but for F1 score, 74.74% is as close as the model got without overfitting.

The final model can accurately predict whether an individual got the seasonal flu vaccine about 77% of the time.

## Limitations and Next Steps
### Limitations
The dataset used in training these models exhibits significant bias towards certain demographics, such as white individuals and those with higher levels of education, employment status, and income. This bias can lead to skewed model predictions, as the model may prioritize patterns and relationships that are more prevalent within this specific group. Consequently, the model's performance and generalizability to the broader population may be compromised.

### Next Steps:
* Consider more diversity in data collection to obtain data from a more balanced group of people in terms of race, education and income.

* Monitor model performance and retrain the model once more data becomes available.
  
## Recommendation

* Education and Awareness Campaigns: Focus on educating the public about the importance of following preventative guidelines such as frequent hand washing, avoiding large gatherings, and wearing face masks, especially for those who are hesitant about getting vaccinated.

* Emphasize Vaccine Safety and Effectiveness: Highlight the Safety and effectiveness of the flu vaccine in preventing illness and emphasize the risks associated with not getting vaccinated. Focus on educating the public about how vaccines work and addressing any questions people might have about vaccines.

* Encourage healthcare providers to recommend the flu vaccine to their patients, as individuals are more likely to get vaccinated when it is recommended by a doctor. 

* Target Specific Demographic Groups: Tailor outreach efforts to demographic groups that are less likely to be vaccinated, such as younger individuals and those with lower levels of education.

* Ensure that cost is not a barrier to vaccination by offering free or low-cost vaccination clinics, particularly for individuals with lower incomes. 

