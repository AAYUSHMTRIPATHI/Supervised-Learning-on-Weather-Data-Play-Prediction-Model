# 🌦️ Play Weather Classification using Decision Trees

## 📌 Project Overview

This project implements a Decision Tree classifier to predict whether an outdoor activity (Play) should occur based on weather conditions.

The objective is to:

- Apply supervised classification on a small structured dataset
- Understand how Decision Trees work
- Analyze the impact of duplicate records on model performance
- Compare model behavior on datasets with and without duplicate values

---

## 📂 Dataset Description

The dataset contains weather-related features:

- Outlook (Sunny, Overcast, Rain)
- Temperature (Hot, Mild, Cool)
- Humidity (High, Normal)
- Wind (Weak, Strong)
- Target Variable: Play (Yes / No)

Two versions of the dataset were used:

1. Dataset containing duplicate rows
2. Dataset with duplicate rows removed

---

## 🎯 Problem Statement

Given weather conditions, predict whether the activity should be played or not.

This is a **binary classification problem**.

---

## 🤖 Model Used

A **Decision Tree Classifier** was implemented.

Decision Trees were chosen because:

- They are easy to interpret
- They work well with categorical data
- They require minimal preprocessing
- They visually demonstrate how decisions are made

---

## 🔬 Why Two Decision Trees Were Built

Two separate Decision Tree models were trained:

### 1️⃣ Model Trained on Dataset WITH Duplicate Values

This dataset includes repeated records of the same weather conditions and outcomes.

Purpose:
- To observe how duplicates influence the decision boundaries
- To understand how repeated examples impact feature importance
- To evaluate potential bias caused by repeated samples

Effect of Duplicates:
- The model may give higher importance to patterns that appear more frequently
- Repeated records increase weight implicitly
- Tree splits may become biased toward duplicated patterns

---

### 2️⃣ Model Trained on Dataset WITHOUT Duplicate Values

This dataset removes repeated entries.

Purpose:
- To observe the true underlying decision structure
- To eliminate artificial weighting caused by repeated samples
- To compare structural differences in the generated tree

Effect of Removing Duplicates:
- Each unique pattern contributes equally
- Model becomes less biased toward repeated conditions
- The tree structure may simplify

---

## 📊 Key Comparison

By training two models, we were able to analyze:

- Differences in tree depth
- Differences in splitting criteria
- Changes in feature importance
- Variations in classification accuracy

This comparison demonstrates how dataset quality and preprocessing decisions influence machine learning models.

---

## 🧠 Key Insights

- Duplicate records can unintentionally bias machine learning models.
- Decision Trees are sensitive to frequency patterns in the data.
- Removing duplicates can lead to more generalized decision boundaries.
- Data preprocessing decisions significantly affect model behavior.

---

## 📌 Learning Outcomes

This project demonstrates:

- Supervised learning fundamentals
- Decision Tree implementation
- Importance of data cleaning
- Impact of duplicates on classification models
- Model comparison techniques

---

## 🚀 Future Improvements

- Compare with Naive Bayes classifier
- Perform cross-validation
- Visualize tree structures
- Analyze feature importance numerically
- Introduce pruning techniques

---

