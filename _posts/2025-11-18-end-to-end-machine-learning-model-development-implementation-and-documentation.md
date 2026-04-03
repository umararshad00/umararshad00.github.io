---
title: "End-to-End Machine Learning Model Development, Implementation, and Documentation"
layout: post
subtitle: "This project phase brought together data preprocessing, feature engineering, model training, evaluation, and report writing into one complete workflow."
topics:
  - Regression Project
  - Random Forest
  - Technical Documentation
points:
  - Selecting a regression dataset and defining the prediction problem
  - Building the workflow through preprocessing, visualization, and feature engineering
  - Training, evaluating, selecting the final model, and documenting the project
---

After understanding data visualization and model evaluation, I moved into the most important part of my project: the full implementation of a machine learning model. For this stage, I selected the PakWheels Used Car Dataset, where the main objective was to predict car prices. Since the project involved continuous values, it naturally became a regression problem.

This dataset gave me the chance to work on a practical, real-world task rather than a purely academic example. It helped me understand how machine learning can be used to solve problems that people actually care about, such as estimating the value of a used car based on its features.

I approached the project in a structured and step-by-step way. First, I imported the necessary libraries and loaded the dataset into my working environment. Then I began exploring the data and identifying issues such as missing values. Handling these issues carefully taught me how important data preprocessing is to the quality of the final model.

Once the data became cleaner, I created visualizations to better understand patterns and relationships in the dataset. After that, I performed feature encoding, especially One-Hot Encoding, so that categorical variables could be converted into numerical form. This step was essential because machine learning algorithms require numeric input.

Next, I divided the data into training and testing sets using the train-test split method. This allowed me to train models on one portion of the dataset and then evaluate them on unseen data. That separation was important for understanding whether the model could generalize instead of simply memorizing the data.

For model selection, I explored Logistic Regression, Decision Tree, and Random Forest. Logistic Regression was included mainly for learning purposes, while Decision Tree and Random Forest were more suitable for the regression task. After training the models, I evaluated them using MSE, RMSE, and R2 Score.

When I compared the results, Random Forest gave the strongest performance, so I selected it as my final model. I also created a scatter plot of actual versus predicted prices, which visually showed how closely the model's output matched the real values. That chart gave me a clearer sense of how well the final solution was working.

In addition to coding, I prepared a detailed project report of around 15 to 20 pages. In that report, I explained the purpose of each section of the code, the workflow I followed, and the reasoning behind my decisions. This documentation phase strengthened my ability to communicate technical work clearly, and it reminded me that good projects require not only implementation, but also explanation.
