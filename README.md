# Project Name : NLP - Automatic Ticket Classification case study

## Table of Contents
* [General Info](#general-information)
* [Steps](#pipelines)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)
  

## General Information
> You need to build a model that is able to classify customer complaints based on the products/services. By doing so, you can segregate these tickets into their relevant categories and, therefore, help in the quick resolution of the issue.

> You will be doing topic modelling on the <b>.json</b> data provided by the company. Since this data is not labelled, you need to apply NMF to analyse patterns and classify tickets into the following five clusters based on their products/services:

* Credit card / Prepaid card

* Bank account services

* Theft/Dispute reporting

* Mortgages/loans

* Others


> With the help of topic modelling, you will be able to map each ticket onto its respective department/category. You can then use this data to train any supervised model such as logistic regression, decision tree or random forest. Using this trained model, you can classify any new customer complaint_what_happened support ticket into its relevant department.

## Pipelines

> You need to perform the following eight major tasks to complete the assignment:

1.  Data loading

2. Text preprocessing

3. Exploratory data analysis (EDA)

4. Feature extraction

5. Topic modelling

6. Model building using supervised learning

7. Model training and evaluation

8. Model inference

## Conclusions

#### Inference:

| Model                   | Accuracy   | Key Observations                                                                                                                                                       |
| ----------------------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Logistic Regression** | **0.9381** | - Highest accuracy among all models<br>- Precision, recall, and F1-scores are consistently high across all classes<br>- Balanced performance: ideal for production use |
| **Decision Tree**       | 0.7772     | - Performs significantly worse than Logistic Regression<br>- Lower precision and recall across most classes<br>- Likely overfitting/underfitting issues                |
| **Random Forest**       | 0.8418     | - Good balance between precision and recall for classes 0–3<br>- Slight drop in recall for class 4 (0.587)<br>- Better generalization than a single decision tree      |
| **Naive Bayes**         | 0.8225     | - Performs well for classes 0–2<br>- Struggles with class 4 (lower precision)<br>- Simple and efficient but not the most accurate                                      |

##### Performance Summary

- Logistic Regression is the best performing model, achieving the highest overall accuracy (93.8%) with strong class-wise precision, recall, and F1-scores.

- Random Forest is a strong runner-up, with robust performance and less overfitting than Decision Trees.

- Naive Bayes offers decent results with faster computation, making it suitable for quick baselines or resource-constrained environments.

- Decision Tree alone is not recommended due to lower accuracy and potential overfitting.


## Technologies Used
- Python - version 3.12.4
- Pandas - version 2.2.2
- Numpy
- Json
- Joblib
- Spacy
- en_core_web_sm
- tqdm
- wordcloud 1.9.4
- GoogleColab
- Matplotlib - version 3.8.4
- Seaborn - version 0.13.2
- Sklearn
- Jupyter Notebook
- Anaconda Navigator 2.6.3
- Visual Studio Code 1.96.0



## Acknowledgements
- I would like to express gratitude to the UpGrad and IIITB Programme for providing me with the opportunity to implement NLP as part of our coursework. 
- This case study has enriched our understanding and practical application of data analysis techniques, contributing significantly to our learning experience.


## Contact
Created by [@niranjantitan]


## License
This project is open source and available without restrictions.
