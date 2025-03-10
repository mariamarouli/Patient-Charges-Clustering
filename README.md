# Patient Charges Clustering and Prediction

## Overview
This project focuses on analyzing the insurance charges of patients using various machine learning techniques. We aim to explore patterns in the dataset, perform clustering to group similar patients, and use Linear Regression for predicting patient charges. The dataset includes patient information such as age, sex, bmi (Body Mass Index), children (number of children/dependents), smoker status, region, and charges.

## Problem Statement
Given a dataset containing various patient characteristics, the goal is to:

* Perform Exploratory Data Analysis (EDA) to understand the data.
* Use K-Means and Gaussian Mixture Model (GMM) to identify clusters of patients with similar insurance charges.
* Build a Linear Regression model to predict insurance charges based on patient attributes.

## Dataset
The dataset used in this project is the insurance.csv file, which contains the following columns:

* age: Age of the patient.
* sex: Gender of the patient (male/female).
* bmi: Body Mass Index (BMI) of the patient.
* children: Number of children/dependents covered by the insurance.
* smoker: Whether the patient is a smoker (yes/no).
* region: The region where the patient lives (northeast, southeast, southwest, northwest).
* charges: The insurance charges for the patient.

## Approach

### 1. Exploratory Data Analysis (EDA)
EDA is used to understand the distribution of the dataset, identify any outliers or missing values, and visualize key relationships between the features and the target variable (charges). This step includes:

* Descriptive statistics.
* Data visualization using histograms, box plots, and bar plots.

### 2. Clustering Patients
We apply two clustering algorithms to group similar patients based on their attributes:

**2.1 K-Means Clustering**
K-Means is used to partition the data into clusters based on patient characteristics (such as age, BMI, smoker status).
We determine the optimal number of clusters using the Elbow Method.

**2.2 Gaussian Mixture Model (GMM)**
GMM is a probabilistic model that assumes the data is generated from a mixture of several Gaussian distributions. We use GMM to cluster patients based on their features and charge distributions.

**3. Linear Regression for Prediction**
Using the clusters identified in the previous step, we build a Linear Regression model to predict charges. The model is trained using the following features:

* age
* sex
* bmi
* children
* smoker
* region


The model is evaluated using mean squared error (MSE) and R-squared to assess the accuracy of the predictions.

