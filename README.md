# Kaspi Lab task / Salary in Kazakhstan

This repo contains my solution for the [Kaspi Lab task](https://www.kaggle.com/c/salarykz). The idea is to predict a salary given a job position and test results.

## Problem statement

You are provided with specialists with a list of grades received at the university and salaries they receive. You need to predict the salaries of other workers based on the same data.

The data is completely synthetic. They have a pattern that needs to be determined, but all the numbers are randomly generated. So any coincidences with real people are just coincidences.

## Model evaluation

I used a pipeline with a standard scaler, polynomial features and a linear regression without regularization. It showed an RMSE score of 50791.66 on the testing dataset, ranking 22th best out of 219 participants.

## Project structure

    .
    ├── final_predict.csv              # submission file with predictions
    ├── kaspi_lab.ipynb                # main .ipynb code file
    ├── models.joblib                  # dictionary with pipelines of models
    ├── salary_example_submition.csv   # sample of submission file
    ├── salary_predict.csv             # testing dataset
    ├── salary_train.csv               # training dataset
    └── README.md
