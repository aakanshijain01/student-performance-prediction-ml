Project Overview

Student Performance Prediction System using Machine Learning is a beginner-friendly machine learning project developed as part of the VITyarthi Build Your Own Project initiative. The main purpose of this project is to develop a system that can predict a student's final academic result as Pass or Fail based on several academic and behavioral factors.

The project focuses on a common problem faced by students and teachers: it can be difficult to estimate a student's final academic performance by looking at individual academic factors separately. Factors such as study hours, attendance, previous marks, assignment scores, and internal marks can provide useful information about a student's overall performance. This project combines these factors and uses a machine learning classification model to generate a predicted result.

The system uses a Decision Tree Classifier for prediction. The model is trained using a sample student dataset stored in dataset.csv. After training, users can enter the details of a new student through either the Python-based prediction program or the Streamlit web application. The trained model then predicts whether the student is likely to Pass or Fail.

The project also includes an analysis module that calculates basic statistics from the dataset and generates a graphical representation of the student result distribution. This makes the project more than just a prediction program and demonstrates different stages of a machine learning application, including data input, data processing, model training, prediction, evaluation, testing, and visualization.

Problem Statement

Students' academic performance is influenced by multiple factors. A student's study hours, attendance, previous academic marks, assignment performance, and internal assessment marks can all provide information about their academic progress.

However, manually analyzing these factors and estimating the final result can be time-consuming. A simple machine learning system can help process these factors together and provide a predicted outcome.

The objective of this project is therefore to create a Student Performance Prediction System that accepts relevant student information and uses machine learning to predict the student's final result as Pass or Fail.

The project is intended as an educational demonstration of how machine learning can be applied to a real-world academic prediction problem.

Objectives

The major objectives of the project are:

To develop a machine learning-based student performance prediction system.
To use academic and behavioral features for prediction.
To implement a Decision Tree Classification model.
To provide an easy method for entering student information.
To predict the student's final result as Pass or Fail.
To evaluate the machine learning model using test data.
To provide basic statistical analysis of the student dataset.
To generate a visualization of the result distribution.
To provide a simple web-based interface using Streamlit.
To demonstrate software development practices such as modular programming and basic testing.
Main Features

The GitHub project contains several important features.

1. Student Data Input

The system accepts the following student information:

Study Hours
Attendance
Previous Marks
Assignment Score
Internal Marks

These values are used as input features for the machine learning model.

2. Data Processing

The project reads the student dataset from dataset.csv using Pandas. The data is# student-performance-prediction-ml
