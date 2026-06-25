---
title: "Model Training, Evaluation, and Project Documentation"
layout: post
sequence: 10
blog_category: first-semester
subtitle: "The second half of my machine learning project: training models, selecting Random Forest, and documenting the complete workflow."
image: "/assets/images/post-scenes/fresh-start-class.jpg"
image_alt: "Students working in a bright classroom while preparing a technical project"
image_caption: "A focused classroom scene that fits model training and project documentation"
image_credit: "Photo via Pexels"
topics:
  - Model Training
  - Random Forest
  - Documentation
points:
  - Splitting data into training and testing sets
  - Comparing Logistic Regression, Decision Tree, and Random Forest
  - Preparing a detailed project report and final documentation
---

## Training and Testing the Models

Next, I divided the dataset into training and testing sets using the train-test split method. This allowed me to train the model on one portion of the data and test its performance on unseen data, ensuring that the model generalizes well. After preparing the data, I moved towards model selection, where I experimented with three different algorithms: Logistic Regression, Decision Tree, and Random Forest.

Even though Logistic Regression is generally used for classification problems, I explored it for learning purposes, while Decision Tree and Random Forest were more suitable for my regression task. This comparison helped me understand that model choice should depend on the problem type, dataset, and evaluation results rather than only on popularity.

## Evaluating and Selecting Random Forest

Once the models were selected, I performed model training, where each model learned from the training data. After training, I evaluated the models using appropriate regression metrics, including Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R2 Score. These metrics helped me understand how accurately my model was predicting car prices.

After comparing the performance of all models, I found that the Random Forest model gave the best results. Therefore, I selected it as my final model and saved it for future use. Selecting Random Forest made sense because it performed better than the other approaches I tested. Instead of depending on one decision tree, Random Forest combines multiple trees, which can improve stability and prediction quality.

## Documentation and Portfolio Learning

In addition to coding and implementation, I also prepared a detailed project report consisting of approximately 15 to 20 pages. In this report, I clearly explained each part of my code, describing what every section was doing and why it was important. I also included additional explanations about concepts, methodologies, and results to make the report more comprehensive.

Documentation was almost like revising the whole project again. When I wrote explanations for each section of code, I had to check whether I truly understood it. This made the report more than a formality. It became a learning tool and supported the purpose of my portfolio website. A strong digital footprint is not only made from screenshots or code files. It is built from clear explanations that show what I learned and how I solved problems.

Students can explore Dr. Bilal Ahmad's [Google Scholar profile](https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en) to see how research and model development connect with real academic impact.

#MLwithDrBilalAhmad #DrBilalAhmad #MLProject
