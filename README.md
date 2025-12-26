# Practical Machine Learning – Prediction Assignment

This repository contains my submission for the **Coursera Practical Machine Learning Course Project**.

The objective of this project is to predict the manner in which participants performed barbell lifts using data collected from accelerometers placed on the belt, forearm, arm, and dumbbell.

---

## Files in this Repository

- **prediction_assignment.Rmd**  
  R Markdown file containing the complete analysis, model building, cross-validation, and predictions.

- **prediction_assignment.html**  
  Compiled HTML version of the analysis (for peer review).

- **README.md**  
  This file.

---

## Data

The data used in this project comes from the Practical Machine Learning course on Coursera.

- Training data:  
  https://d396qusza40orc.cloudfront.net/predmachlearn/pml-training.csv

- Test data:  
  https://d396qusza40orc.cloudfront.net/predmachlearn/pml-testing.csv

The original dataset was made available by the Human Activity Recognition research group at PUC-Rio.

---

## Methodology

1. Loaded and cleaned the dataset by removing columns with a high percentage of missing values.
2. Removed non-predictive variables such as identifiers and timestamps.
3. Split the training data into training (70%) and validation (30%) sets.
4. Trained multiple models, including:
   - Decision Tree
   - Random Forest
5. Selected **Random Forest** as the final model due to its high accuracy.
6. Estimated out-of-sample error using cross-validation.
7. Generated predictions for 20 test cases for submission.

---

## Results

- The Random Forest model achieved very high accuracy (approximately 99%).
- The expected out-of-sample error was very low.
- All 20 test cases were successfully predicted and submitted for automated grading.

---

## How to Reproduce

1. Open `prediction_assignment.Rmd` in RStudio.
2. Ensure required packages are installed:
   - caret
   - randomForest
   - rpart
   - rpart.plot
3. Click **Knit → HTML** to generate the report.

---

## Author

**Nishath Anjum**

---

This project is submitted as part of the Coursera Practical Machine Learning course.
