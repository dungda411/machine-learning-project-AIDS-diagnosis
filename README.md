# 🌳 Tree Models in AIDS Diagnosis
-----------------------------------------------------
## Table of contents:
### 1. Introduction
### 2. Project Description
### 3. Result and Discussion
-----------------------------------------------------
# 1. Introduction
With the rise of data, machine learning has played vital roles in many fields, especially healthcare. There have been many research delving into its potential in diseases diagnosis, with promising accuracy. Among conventional algorithms, tree models are proven to performance great in compared to the others (e.g., in financial fraud detection). So, this project aims at evaluating their performances in healthcare, particularly AIDS diagnosis.

-----------------------------------------------------
# 2. Project Description
The dataset used for analysis (published in 1996, available on Kaggle) contains information about 2,139 patients diagnosed with AIDS, and includes 22 independent variables and 1 target. In this project, a full machine learning workflow was implemented:

- First, exploratory data analysis (EDA) aims to learn the dataset and the relationship between features. Visualization was performed, with a variety of chart types, such as histogram, bar chart, box plot, heatmap.
![image](https://github.com/dungda411/machine-learning-project-AIDS-diagnosis/assets/157843205/a966869b-2dad-42fa-a562-fff3c15dbad8)
![image](https://github.com/dungda411/machine-learning-project-AIDS-diagnosis/assets/157843205/16c15cc0-2994-4946-b0e6-e2446ea4c84e)
![image](https://github.com/dungda411/machine-learning-project-AIDS-diagnosis/assets/157843205/79441b31-4156-4d74-a64d-fa75112dccd7)
![image](https://github.com/dungda411/machine-learning-project-AIDS-diagnosis/assets/157843205/9fe4d179-d1c0-4496-8366-63206bfa264e)

- Next, dataset was prepared for the model developments. This step includes cleaning, splitting and engineering features.

- And lastly, 5 models were developed and evaluated, including Random Forest, Gradient Boosting, Extra Trees, Bagging and Voting Classifier. Hyperparameters of each models were tuned with the help of GridSearchCV. The wide range of metrics was used for comparison, with balanced accuracy being the most important, especially for imbalanced dataset.

-----------------------------------------------------
# 3. Result and Discussion
The result shows that Bagging Classifier performs the best with 91.6% accuracy. Looking at the confusion matrix, Extra Trees also has great performance, just slightly lower than Bagging. Moreover, Voting Classifier does better in predicting those that not infected with AIDS.
![image](https://github.com/dungda411/machine-learning-project-AIDS-diagnosis/assets/157843205/2b770c9f-1a13-4120-9dbe-5be653589da0)
However, the question is that, is 91.6% good enough? In the context of healthcare, where the barrier between patient’s life and death is in the hands of care providers, is relying on machine a good idea? Is it ethical? Many researchers have discussed about the term ‘explainability’ in machine learning. My point of views on this topics will be blogged as I am diving into it for my dissertation. Stay tuned!
