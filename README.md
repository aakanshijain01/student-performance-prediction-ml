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
organized into input features and the target variable.

The five main input features are:

study_hours
attendance
previous_marks
assignment_score
internal_marks

The target variable is:

final_result

which contains the student's final result.

3. Machine Learning Prediction

The project uses a Decision Tree Classifier from Scikit-learn.

The model learns patterns from the available student records and uses those patterns to classify a new student's result as:

Pass

or

Fail
4. Model Evaluation

The project divides the available data into training and testing portions.

The model is trained using the training data and then tested using previously unseen test records. The project calculates model accuracy using accuracy_score.

During the current test run, the sample dataset produced an accuracy of 1.0 on its test split. However, the dataset contains only 20 sample records, so this result should not be interpreted as evidence of real-world predictive performance.

5. Web Application

The project includes a Streamlit application in:

app.py

The application provides a simple interface where a user can enter student details and click Predict Result.

The system then displays:

Predicted Result: PASS

or

Predicted Result: FAIL

This makes the machine learning model easier to demonstrate than using only the command line.

6. Data Analysis and Visualization

The project contains:

analysis.py 📊

This module performs basic statistical analysis of the dataset.

It calculates values such as:

Total number of students
Average study hours
Average attendance
Average previous marks
Average assignment score
Average internal marks
Number of Pass students
Number of Fail students

It also creates a bar chart showing the distribution of Pass and Fail results.

The generated chart is saved as:

student_result_chart.png
Dataset

The project currently uses a small sample dataset named:

dataset.csv

The dataset contains 20 student records.

It includes the following columns:

Column	Description
study_hours	Number of hours spent studying
attendance	Student attendance percentage
previous_marks	Previous academic marks
assignment_score	Assignment performance
internal_marks	Internal assessment marks
final_result	Final Pass/Fail result

The current dataset contains:

12 Pass records
8 Fail records

The calculated averages are approximately:

Average Study Hours: 3.65
Average Attendance: 73.5%
Average Previous Marks: 63.0
Average Assignment Score: 68.75
Average Internal Marks: 65.1

Because this is a small sample dataset, it is mainly intended for demonstration and educational purposes.

Machine Learning Model

The project uses the Decision Tree Classifier.

A Decision Tree is a supervised machine learning algorithm that makes predictions by creating decision rules based on the input features.

In this project, the model receives information such as:

Study Hours
Attendance
Previous Marks
Assignment Score
Internal Marks

and predicts:

Pass / Fail

The Decision Tree model was selected because it is relatively easy to understand and is suitable for a beginner-level classification project.

The model is implemented using:

scikit-learn
System Workflow

The overall system works approximately as follows:

Student
   ↓
Enter Student Details
   ↓
Streamlit Web Application
   ↓
Data Processing
   ↓
Decision Tree Machine Learning Model
   ↓
Pass / Fail Prediction
   ↓
Display Result

The project also contains a separate analysis process:

dataset.csv
     ↓
analysis.py
     ↓
Statistical Analysis
     ↓
Student Result Chart
Project Architecture

The system is divided into several logical components.

Student

The student provides the required academic information.

Streamlit Application

app.py provides the graphical/web interface for entering student information.

Dataset

dataset.csv contains the sample student records used for training and testing.

Machine Learning Model

The Decision Tree Classifier learns from the dataset and performs classification.

Prediction Module

prediction.py allows student information to be entered through the Python program and generates a Pass/Fail prediction.

Analysis Module

analysis.py calculates dataset statistics and generates a visualization.

Testing Module

test_model.py performs basic checks to verify that the dataset and prediction functionality are working correctly.

Important Project Files

The repository contains multiple files, each serving a specific purpose.

app.py

This is the main Streamlit web application.

It:

Loads the dataset
Prepares the features
Trains the Decision Tree model
Accepts student information
Performs prediction
Displays the result
model.py

This file contains the main model-training and prediction implementation.

It also calculates the model accuracy on the test data.

prediction.py

This provides a command-line version of the prediction system.

The user enters the five student features directly into the terminal and receives a Pass/Fail prediction.

analysis.py 📊

This module performs statistical analysis and creates the student result distribution chart.

dataset.csv

This is the sample dataset used by the machine learning system.

test_model.py

This contains basic tests for:

Dataset availability
Required columns
Model prediction functionality
requirements.txt

This file lists the Python libraries required by the project, including:

pandas
scikit-learn
matplotlib
streamlit
joblib
README.md

The README provides project documentation, including:

Project overview
Objectives
Features
Technologies
Installation instructions
Running instructions
Dataset information
Limitations
Future enhancements
statement.md

This document contains the formal problem statement, project objective, target users, and high-level features.

Technologies Used

The project uses the following technologies:

Python

Python is the primary programming language used to implement the machine learning system.

Pandas

Pandas is used for loading, processing, and analyzing the CSV dataset.

Scikit-learn

Scikit-learn is used to implement:

Decision Tree Classifier
Train-test splitting
Accuracy evaluation
Matplotlib

Matplotlib is used to generate the student result distribution chart.

Streamlit

Streamlit is used to create the interactive web interface.

GitHub

GitHub is used to store and document the project source code and project resources.

Testing

Basic testing has been included through:

test_model.py

The testing module verifies that:

The dataset contains records.
Required columns exist.
The machine learning model can be trained.
The model can generate a valid Pass/Fail prediction.

The current basic test run produced:

All basic tests passed successfully!

This provides a basic level of confidence that the main dataset and prediction functionality are working as expected.

Example Prediction

For demonstration, the system was tested with a student having:

Study Hours       = 5
Attendance        = 85
Previous Marks    = 75
Assignment Score  = 80
Internal Marks    = 78

The system generated:

Predicted Result: PASS

This demonstrates how a new student's information can be supplied to the trained model to obtain a prediction.

Visualization

The analysis module creates a result distribution chart.

The chart represents the number of:

Pass students
Fail students

in the current sample dataset.

This provides a simple visual understanding of the dataset and demonstrates the use of data visualization alongside machine learning.

Project Diagrams

The project documentation includes several diagrams to describe the system design:

System Architecture Diagram

Shows the overall flow between the student, Streamlit application, data processing, machine learning model, prediction, and result display.

Use Case Diagram

Shows the interaction between the student and the major functions of the system, such as entering student details, predicting performance, viewing prediction, and viewing analysis.

Class Diagram

Shows the major logical components/classes involved in the system and their relationships.

Sequence Diagram

Shows the sequence of interactions between the student, Streamlit application, dataset, Decision Tree model, and analysis module during system operation.

These diagrams help explain the design and architecture of the project in a structured way.

Advantages of the Project

The project demonstrates several useful concepts:

Simple and understandable machine learning workflow
Easy student data input
Automated Pass/Fail prediction
Interactive web interface
Dataset analysis
Visualization
Basic software testing
Modular Python files
GitHub-based project documentation
Clear system architecture and UML documentation

It also provides a practical example of how a machine learning model can be integrated into a simple software application.

Limitations

The current project has some important limitations.

Small Dataset

The project currently uses only 20 sample records. A larger and more diverse dataset would be needed for meaningful real-world evaluation.

Synthetic/Demonstration Data

The current dataset is intended for project demonstration and does not represent the complete student population.

Limited Prediction Categories

The current system predicts only:

Pass
Fail

It does not currently predict specific grades or marks.

Limited Features

Only five main factors are used:

Study hours
Attendance
Previous marks
Assignment score
Internal marks

Other potentially relevant factors are not currently included.

Model Limitations

Only a Decision Tree model is currently implemented. Other algorithms have not yet been compared systematically.

Therefore, the current model accuracy should be treated as a demonstration result rather than a reliable real-world performance measurement.

Future Enhancements

The project can be extended in several ways.

1. Larger Dataset

A larger real-world or appropriately sourced educational dataset could be used to improve the evaluation of the system.

2. More Machine Learning Models

Future versions could compare different classification algorithms, such as:

Logistic Regression
Random Forest
Support Vector Machine
K-Nearest Neighbors

Model performance could then be compared using appropriate evaluation metrics.

3. Grade Prediction

Instead of only predicting Pass/Fail, the system could be extended to predict categories such as:

Excellent
Good
Average
Needs Improvement
4. More Student Factors

Additional features could be considered, such as:

Number of completed assignments
Previous semester performance
Study consistency
Subject-wise marks
5. Improved Visualization

The web application could include more charts showing relationships between academic factors and student results.

6. Database Integration

Instead of storing data only in a CSV file, a future version could use a database to store student records.

7. Authentication

A future version could provide separate access for students and teachers.

8. Performance Monitoring

The system could be extended to identify students who may need additional academic support based on their performance indicators.

Conclusion

The Student Performance Prediction System using Machine Learning demonstrates the development of a complete beginner-level machine learning application. The project starts with student data, processes relevant academic features, trains a Decision Tree classification model, and uses the model to predict whether a student is likely to pass or fail.

The project also demonstrates how a machine learning model can be integrated into a user-friendly Streamlit web application. In addition, the analysis module provides statistical information and visualization of the dataset, while the testing module verifies basic system functionality.

From a software-development perspective, the project covers several important areas, including problem identification, functional modules, machine learning, data processing, prediction, visualization, testing, documentation, system architecture, UML diagrams, and GitHub-based project management.

The current version is primarily an educational prototype because it uses a small sample dataset. Nevertheless, it provides a foundation that can be expanded with a larger dataset, additional features, multiple machine learning models, improved evaluation, database integration, and a more advanced user interface.

Overall, the project demonstrates how machine learning concepts can be combined with Python programming and web technologies to create a practical Student Performance Prediction System suitable for academic project demonstration and further development.
