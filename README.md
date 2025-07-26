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

| Model                     | Accuracy  | Macro F1  | Comments                                                                   |
| ------------------------- | --------- | --------- | -------------------------------------------------------------------------- |
|**Logistic Regression** | **0.940** | **0.939** | Best performing model — high, balanced precision/recall across all classes |
| Random Forest             | 0.836     | 0.830     | Good performance, slight dip in class consistency                          |
| Naive Bayes               | 0.821     | 0.809     | Decent; overestimates some classes, underperforms on others                |
| Decision Tree             | 0.785     | 0.777     | Weakest overall — unstable class-wise recall/precision                     |

##### Performance Summary

1. **Logistic Regression (Best Performing Model)**

    Achieves consistently high precision, recall, and F1-scores across all classes.

    Well-balanced model and ideal for deployment in its current state.

    Recommended as the final model for the task.

2. **Random Forest (Good Alternative)**

    Performs well but slightly inconsistent across classes (notably lower precision for class 4).

    Could be enhanced with hyperparameter tuning or class balancing.

    Suitable for use if nonlinear relationships are important.

3. **Naive Bayes**

    Decent performance on most classes, but suffers from lower precision in class 4.

    Fast and lightweight, but assumptions of feature independence may limit performance.

4. **Decision Tree (Least Effective)**

    Shows inconsistent performance, especially poor for class 3 recall.

    Likely overfitting or underfitting due to lack of depth control or pruning.

    Not recommended without significant tuning.

##### Final Recommendation

- Use Logistic Regression as the primary model — it's accurate, balanced, and interpretable.

- Optionally, experiment with Random Forest or XGBoost for further performance improvement.

- Ensure class distributions are handled properly (e.g., oversampling, class_weight='balanced') for better generalization.


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
