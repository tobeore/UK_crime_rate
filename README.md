# UK Crime Rate Analysis



## 📌 Project Overview

In recent years, there has been a steady increase in the rate of crimes in the United Kingdom. One major aspect of combating the prevailing high crime rate is making decisions based on the analysis of past data. This project analyzes crime rates in the UK and evaluates machine learning models built to classify crime levels. The findings are intended to be used to recommend actionable solutions to combat the rising crime rate.

## 🎯 Aim & Objectives

The primary aim of this analysis is to gain insights from the data and build a machine learning model capable of classifying an area based on its crime rate.

The core objectives include:

  * To analyze the data to find 5 key insights.
  * To train and evaluate a machine learning model to classify crime levels based on historical patterns.
  * To provide recommendations to help reduce the rising crime rate.

## 📊 Dataset Information

  * **Source**: Police recorded crime Police Force Area Open Data tables from the Home Office.
  * **Timeframe**: Year ending March 2013 to the year ending June 2023.
  * **Size**: 258,905 rows and 8 columns.
  * **Features**: The data consists of 8 features: Financial Year, Financial Quarter, Force Name, Offence Description, Offence Group, Offence Subgroup, Offence Code, and Number of Offences.

## 💡 Key Insights

  * **Yearly Crime Rate**: There was a steady increase in offenses from 2012/13 to 2016/17, followed by a sharper increase from 2016/17 to 2018/19. A slight decrease occurred in 2020/21, which could be attributed to policy changes or data inconsistency.
  * **Offense Rate by Force**: The Metropolitan Police force recorded the highest number of offenses, peaking at 906,112 in 2019/20. The London, City Of force had the least, with its highest at 8,695.0 in 2019/20.
  * **Types of Offences**: Theft offenses have the highest occurrence, followed by "Violence against the person" and "Fraud Offenses".
  * **Fraudulent Related Forces**: There are dedicated forces specifically for fraud-related offenses. This indicates that more efforts are being put in place to handle the high rate of fraud-related activities.
  * **Offence Subgroups**: For "Violence against person" crimes, violence without injury is more common than violence with injury. Homicide has minimal cases, making it the least practiced offense for this category. Business property theft is the least practiced form of theft.

**Summary:** These insights highlight the need for targeted interventions in high-crime regions and improved monitoring of theft-related offenses.

## 🤖 Machine Learning Modeling

For modeling purposes, four features were utilized: Financial Year, Force Name, Number of Offences, and a generated feature named "Crime Force Rate". The generated feature categorized the Force Name into High, Medium, and Low based on quantile ranges and served as the dependent variable.

Two classification models were trained and evaluated:

  * **DecisionTreeClassifier**: Achieved an accuracy of 1.00.
  * **KNeighborsClassifier**: Achieved an accuracy of 1.00, but with slightly lower recall and f1-scores on certain classes.

**⚠️ Note on Model Performance:**
The model achieved very high accuracy (1.00), which suggests possible overfitting or data leakage (likely due to the derivation of the target variable from the input features). Further validation using cross-validation, feature engineering adjustments, and unseen datasets is required to confirm true generalization performance.

Despite this, the **DecisionTreeClassifier** was determined to be the best-performing model for classifying crime levels based on historical patterns.

## 🛠️ Technologies & Libraries Used

  * **Python**
  * **Pandas** (Data manipulation and analysis)
  * **NumPy** (Numerical computing)
  * **Seaborn & Matplotlib** (Data visualization)
  * **Scikit-Learn** (Machine learning algorithms and metrics)

## 🚀 Recommendations

Based on the analysis, the following actions are recommended:

  * **Resource Allocation**: More resources should be allocated to police forces with historically high crime levels.
  * **Social Awareness**: Members of the community should be informed about the crime rates in their areas and awareness should be given on how to avoid becoming victims.
  * **Policy Changes**: New policies should be made or old policies changed to help reduce the prevailing increase in certain offense groups.

## 📁 Repository Structure

  * `Report.pdf`: Comprehensive analysis report detailing the findings, visual insights, and model performance evaluations.
  * `UK_CrimeRate_Analysis.ipynb`: The Jupyter Notebook containing the data scanning, preprocessing, exploratory data analysis, and model training code.
  * `reccrime-offence-ref - Reference_Table_-_Offence.csv`: A reference table mapping specific offense codes to their respective descriptions, groups, and subgroups.
  * `LICENSE`: Details the licensing information for the code.

## 📜 License

This project is licensed under the MIT License. Copyright (c) 2024 tobeore.

## 👤 Author

**Tobechukwu (tobeore)**
