# DonorsChoose Project Proposal Prediction

## Overview

DonorsChoose.org receives hundreds of thousands of project proposals each year for classroom projects in need of funding. Currently, a large number of volunteers is needed to manually screen each submission before it’s approved to be posted on the DonorsChoose.org website. Next year, DonorsChoose.org expects to receive close to 500,000 project proposals. This project aims to address the following challenges:

- How to scale current manual processes and resources to screen 500,000 projects.
- How to increase the consistency of project vetting across different volunteers.
- How to focus volunteer time on the applications that need the most assistance.

The goal of the competition is to predict whether or not a DonorsChoose.org project proposal submitted by a teacher will be approved, using the text of project descriptions as well as additional metadata about the project, teacher, and school.

## Type of Model Used
- LSTM

## Workflow

1. **Data Collection and Preprocessing**: Gathered data on project descriptions, teacher, and school metadata. Preprocessed the text data to prepare it for model training.
2. **Feature Engineering**: Extracted relevant features from the text descriptions using techniques such as CountVectorizer.
3. **Model Training**: Trained various machine learning models to predict whether a project proposal will be approved.
4. **Model Evaluation**: Evaluated the models using the AUC (Area Under the Curve) metric to determine their performance.

| S.NO. | Architecture                    | Test AUC |
|-------|---------------------------------|----------|
| 1     | Model 1                         | 0.7607   |
| 2     | Model 2                         | 0.7149   |
| 3     | Model 3 without CountVectorizer | 0.7634   |
| 4     | Model 3 with CountVectorizer    | 0.7663   |

## Conclusion

The project successfully demonstrates the application of machine learning techniques to predict the approval of DonorsChoose.org project proposals. By leveraging different models and feature engineering techniques, we achieved a test AUC score of up to 0.7663. These models can help in scaling the screening process, increasi
