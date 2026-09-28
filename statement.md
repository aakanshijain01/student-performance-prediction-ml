# Student Performance Prediction System

## 1. Problem Statement

Students' academic performance depends on several factors such as attendance, internal marks, assignment marks, and previous examination marks. It can be difficult to quickly analyze all these factors and identify a student's overall performance.

The **Student Performance Prediction System** is a simple Python-based project that collects student academic information, calculates their total and average marks, and predicts their performance category.

The project is designed using basic programming concepts such as **lists, tuples, dictionaries, functions, conditional statements, loops, arithmetic operations, and file handling**. Student records are stored in a JSON file so that the data can be accessed again when the program is run.

## 2. Scope of the Project

The scope of this project includes:

* Adding and storing student information.
* Recording attendance, internal marks, assignment marks, and previous examination marks.
* Calculating total marks and average marks.
* Predicting student performance based on average marks and attendance.
* Viewing the performance report of an individual student.
* Viewing the performance details of all stored students.
* Saving student data permanently using a JSON file.
* Loading previously saved student records when the program starts.
* Providing a simple menu-driven interface for interaction.

The current project focuses on a **basic rule-based performance prediction system** using Python programming concepts. It does not use advanced machine-learning algorithms.

## 3. Target Users

The main target users of this project are:

* **Students** — to view and understand their academic performance.
* **Teachers** — to quickly review student performance records.
* **Academic users** — to demonstrate basic student performance analysis.
* **Programming students** — to understand the practical application of Python programming concepts.

## 4. High-Level Features

### 1. Student Data Entry

Allows the user to enter student name, attendance, internal marks, assignment marks, and previous examination marks.

### 2. Performance Calculation

Calculates the total marks and average marks of a student using arithmetic operations.

### 3. Performance Prediction

Classifies students into categories such as:

* Excellent Performance
* Good Performance
* Average Performance
* Needs Improvement

The prediction is based on the student's average marks and attendance.

### 4. Individual Student Report

Displays complete academic information, calculated marks, average, and predicted performance for a selected student.

### 5. View All Students

Displays the stored records of all students along with their average marks and performance prediction.

### 6. Data Storage

Stores student information in a `students.json` file so that records are not lost when the program is closed.

### 7. Data Loading

Automatically loads previously saved student records when the application starts.

### 8. Menu-Driven Interface

Provides a simple menu through which users can add students, view reports, view all students, or exit the program.
