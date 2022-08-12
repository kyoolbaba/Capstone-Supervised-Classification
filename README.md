# Capstone-Supervised-Classification
![image](https://user-images.githubusercontent.com/46890041/176097582-427e7ab8-2b60-476a-a72e-1e7a2767d87a.png)


# Company Bankruptcy Prediction
## (Supervised Machine Learning Classification)
### Abstract: Yet we have a classification problem that is related to the Business, Economics, banking sector, We are given data that is collected from the Taiwan economic journal for the year 1999 to 2009 that is company bankruptcy prediction, the company bankruptcy was defined based on the business regulations of the Taiwan Stock Exchange, Getting to know whether a corporate company about its bankruptcy it is a very important economic importance as it affects the stakeholders and the prediction of corporate bankruptcy has been used in most of the studies in Economics accounting and other decision Sciences from past 20 years, therefore, the primary purpose of this prediction is to come up with a model that can give a good prediction about the bankruptcy of the companies

### Problem Statement:
### The prediction of bankruptcy is a phenomenon of increasing interest to firms who stand to lose money because of unpaid debts. Since computers can store huge datasets about bankruptcy making accurate predictions from them beforehand is becoming important.
### The data were collected from the Taiwan Economic Journal for the years 1999 to 2009. Company bankruptcy was defined based on the business regulations of the Taiwan Stock Exchange.
### In this project, you will use various classification algorithms on the bankruptcy datasets to predict bankruptcies with satisfying accuracies long before the actual event.

# Imbalanced Dataset
![image](https://user-images.githubusercontent.com/46890041/176097654-a6560749-a4ab-4e26-8ad9-3bd7a1735891.png)

## Skewness
![image](https://user-images.githubusercontent.com/46890041/176097715-b74f7d00-8d1f-433e-a317-540dda90e7cd.png)


# Splitting Dataset
![image](https://user-images.githubusercontent.com/46890041/176098680-3254f67c-651d-4027-b1e0-bfc85023fee0.png)

# PipeLine
![image](https://user-images.githubusercontent.com/46890041/176098751-3dd7b3f5-bb31-4a3c-9714-f312d18dd3d6.png)

# Hyper tuning with Feature Selection
![image](https://user-images.githubusercontent.com/46890041/176098822-1f1fa657-7034-4068-b175-1c9e1e1b3436.png)

# Process carried before training the model
![image](https://user-images.githubusercontent.com/46890041/176098979-d6bcb7cf-1000-439f-b03d-80a7af2dbecd.png)

# Best Performance
![image](https://user-images.githubusercontent.com/46890041/176099034-f3f3113d-bb5d-413a-8ab0-e7d910aed7ec.png)

# ROC Curve
![image](https://user-images.githubusercontent.com/46890041/176099152-4b000f69-0395-425c-9542-92b06e8d0097.png)

# PRC Curve
![image](https://user-images.githubusercontent.com/46890041/176099195-6a870bb4-f4a5-41b5-819a-58cf93f477b7.png)

# XGBoost Classifier (giving best results)
XGBoost is a decision-tree-based ensemble Machine Learning algorithm that uses a gradient boosting framework. In prediction problems involving unstructured data (images, text, etc.) artificial neural networks tend to outperform all other algorithms or frameworks. However, when it comes to small-to-medium structured/tabular data, decision tree based algorithms are considered best-in-class right now. Please see the chart below for the evolution of tree-based algorithms over the years.
![image](https://user-images.githubusercontent.com/46890041/184294363-ac375ffa-37bd-4dc1-95fe-0ad30f941150.png)
Why does XGBoost perform so well?
XGBoost and Gradient Boosting Machines (GBMs) are both ensemble tree methods that apply the principle of boosting weak learners (CARTs generally) using the gradient descent architecture. However, XGBoost improves upon the base GBM framework through systems optimization and algorithmic enhancements.
![image](https://user-images.githubusercontent.com/46890041/184294454-574076df-6cbc-445e-87df-a2eaa83d83ad.png)

System Optimization:

Parallelization: XGBoost approaches the process of sequential tree building using parallelized implementation. This is possible due to the interchangeable nature of loops used for building base learners; the outer loop that enumerates the leaf nodes of a tree, and the second inner loop that calculates the features. This nesting of loops limits parallelization because without completing the inner loop (more computationally demanding of the two), the outer loop cannot be started. Therefore, to improve run time, the order of loops is interchanged using initialization through a global scan of all instances and sorting using parallel threads. This switch improves algorithmic performance by offsetting any parallelization overheads in computation.
Tree Pruning: The stopping criterion for tree splitting within GBM framework is greedy in nature and depends on the negative loss criterion at the point of split. XGBoost uses ‘max_depth’ parameter as specified instead of criterion first, and starts pruning trees backward. This ‘depth-first’ approach improves computational performance significantly.
Hardware Optimization: This algorithm has been designed to make efficient use of hardware resources. This is accomplished by cache awareness by allocating internal buffers in each thread to store gradient statistics. Further enhancements such as ‘out-of-core’ computing optimize available disk space while handling big data-frames that do not fit into memory.

![image](https://user-images.githubusercontent.com/46890041/184294556-75b63d79-bae2-497c-8bec-962eb2b72cba.png)


# 🏵️: Execution Instructions
1. Step-1 Create a folder 
2. Step -2 Download the dataset into the folder from this kaggle page https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction 
3. Dpwnload the jupyter note boook into the folder 

# 🍷: Credits
MILAN GOWDA J.P.  | Avid Learner | Data Scientist | Machine Learning Engineer | Deep Learning enthusiast

Contact me for Data Science Project Collaboration

[![image](https://user-images.githubusercontent.com/46890041/184296771-50e87d3f-aaec-45a6-9af9-103271288bd2.png)](https://www.linkedin.com/in/milangowda/)

# :books: References  
Krishna Naik Github and Youtube Reference 
https://github.com/krishnaik06/Handle-Imbalanced-Dataset
https://www.youtube.com/watch?v=YMPMZmlH5Bo

Josh Stammer Youtube
https://www.youtube.com/c/joshstarmer

5 Techniques to Handle Imbalanced Data For a Classification Problem
https://www.analyticsvidhya.com/blog/2021/06/5-techniques-to-handle-imbalanced-data-for-a-classification-problem/

