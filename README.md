**🍽️ Classification Model in RStudio – Yelp Cuisine Authenticity**

Built a classification model in **RStudio** to determine the authenticity of cuisines using Yelp restaurant data. The JSON dataset underwent extensive **data cleaning, preprocessing, and manipulation**. Applied **Principal Component Analysis (PCA)** to reduce dimensionality and remove redundancy. Selected key features via **correlation plots** and split data into training, validation, and test sets. Utilized the **Random Forest algorithm** to classify cuisine authenticity based on predictors such as **cuisine type, ratings, and city**.

**🗂️ Dataset Description**
Source: **Yelp Academic Dataset (JSON format)**

Size: Includes thousands of restaurant records across different cuisines and locations

Key Features:

 -Cuisine Type

 -Restaurant Ratings

 -Location (City)

 -Review Counts

Other metadata like attributes and categories

**🔧 Tools & Technologies**:
Programming Language: R

IDE: RStudio

Libraries Used:

 -jsonlite – for importing JSON data

 -dplyr, tidyr – for data cleaning & manipulation

 -ggplot2 – for data visualization

 -caret, randomForest – for modeling

 -corrplot – for PCA and correlation analysis

**🧹 Data Processing Steps**
**Data Import: Parsed large JSON Yelp dataset using jsonlite::fromJSON()**

**Data Cleaning**:

 -Removed nulls and irrelevant attributes

 -Filtered dataset to focus on food-related businesses

 -Data Preprocessing:

 -Converted categorical variables to factors

 -Normalized and scaled numerical features

**Feature Engineering**:

 -Created new columns (e.g., binary flag for cuisine authenticity)

 -Selected features based on business rules and correlation

**📊 Exploratory Data Analysis (EDA)**
 -Visualized distribution of ratings and review counts across cities and cuisine types

 -Generated correlation matrices to identify multicollinearity

 -Performed Principal Component Analysis (PCA) to reduce dimensionality and eliminate redundant variables

**🧠 Model Building**
 -Split dataset into training, validation, and testing sets

 -Chose Random Forest as the primary classifier for its performance on categorical features and interpretability

Input Features:

 -Cuisine type

 -Rating

 -City

 -Review count, etc.

 -Output Target:

 -Authentic vs Non-authentic cuisine flag

**✅ Evaluation Metrics**
Accuracy

Confusion Matrix

ROC Curve

Feature importance ranking (from Random Forest model)


