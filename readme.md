# **Contextualizing Bank Churn**

---

This is a topic chosen for Project 3 on Classification, for the Metis Data Science Bootcamp - Summer 2020 Cohort.

## Context

Churn is a common business problem in many industries. Can we classify churners in a bank's customer dataset and build a model to save costs?

## Goal

Use a model to classify churners and non-churners, find the features most important to classification, then performm cost-benefit analysis to see how effective our model is.

## Findings

Age, number of products, member activity level, and nationality were the characteristics that gave the greatest predictive power in churners. 
Providing extra resources or running promotions for potential churners can have greater long-term business benefits despite initial costs.

# Methodology

## Gathering data:

Data was downloaded from Kaggle: https://www.kaggle.com/shrutimechlearn/churn-modelling

Columns in data were renamed and organized. Only categories that could be used in the modeling process was kept. Data was normalized.


## Exploring and modeling data:
Correlations between customer exits(churn) was found using a correlation plot, and then various charts were used to build understanding of what features might be important for modeling.
Models used were Logistic Regression, K-Nearest Neighbors, Random Forest, Naive Bayes, and XGBoost.

Cost-benefit analysis weighed the churners & non-churners in each confusion matrix to an 80%/20% split, then applied assumptions from CustomerThink that a churner would cost a business $200 annually, and customers who stay would earn $150 annually. We used a hypothetical figure that $100 spent by the bank would retain any customer(earning $50 overall).
For each confusion matrix:
Correctly redicted churners(TP) would earn $50
Missed churners(FN) would lose $200
Correctly predicted non-churners(TN) would earn $150
Missed non-churners(FP) would earn $50.

After weighing a confusion matrix from proportions in the test set(n=2,000) to 80%/20%, the numbers were multiplied by 5 to examine it on a hypothetical 10,000 customers, then the profits/losses for customer situations were accounted for accordingly to find the overall profit from each model confusion matrix.

# Deliverables

* [Full data and analysis](data_and_analysis)
  * [Part 1 - Cleaning](data_and_analysis/Contextualizing_Bank_Churn_-_Part_1_-_Cleaning.ipynb)
  * [Part 2 - EDA](data_and_analysis/Contextualizing_Bank_Churn_-_Part_2_-_EDA.ipynb)
  * [Part 3 - Modeling](data_and_analysis/Contextualizing_Bank_Churn_-_Part_3_-_Modeling.ipynb)
  * [Cost-Benefit Analysis](https://docs.google.com/spreadsheets/d/1rBn8SwVQGSXrwWjoIRNXUXZuQ2Oykt6W2xxqY9QXW9Q/edit?usp=sharing)
* Presentation Deck
  * [PDF version](presentation/Joseph_Grovers-Project_3_-_Contextualizing_Bank_Churn.pdf.zip)
  * [Google Slides version](https://docs.google.com/presentation/d/1o_mITRV8W_pyJ9eRFGMIPwqb17INJqy7qPLSIrmOE24/edit?usp=sharing)
  * [PPT version](presentation/Joseph_Grovers-Project_3_-_Contextualizing_Bank_Churn.pptx.zip)

### [Joseph Grovers GitHub](https://github.com/josephgrovers)

## Technologies Used

* Jupyter Notebook

* Python

* Pandas

* Matplotlib

* Seaborn

* SKLearn

* Numpy

* Google Slides

## Presentation Materials Used

* Slidesgo - Template
* Flaticon - Icons
* Freepik - Infographics & images



