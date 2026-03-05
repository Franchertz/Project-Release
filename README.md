# PROJECT TITLE

### PREDICTIVE RISK MODEL FOR YOUTH RECIDIVISM

### EXECUTIVE SUMMARY

This project develops a machine learning model to identify youth at risk of re-offending within the Ontario youth justice system. 

Early identification of high-risk individuals allows case workers to prioritize intervention programs and allocate resources more effectively.

The project demonstrates how predictive analytics could support evidence-based decision-making in youth justice policy.

## POLICY CONTEXT

Youth reoffending presents operational and social challenges across Ontario’s justice system. 

Data-driven insights can assist government agencies in identifying patterns that may help reduce recidivism.

This project demonstrates how analytics could support decision-making within agencies such as the Ontario Ministry of Children, Community and Social Services.


## DATASET

The prototype uses a synthetic / de-identified dataset representing male youth records from a youth justice setting.

Dataset characteristics

    •	70 youth records

    •	18 structured variables

    •	Mix of behavioural, criminal history, and social indicators

Example variables:

    •	prior violent offence

    •	prior charges count

    •	prior convictions count

    •	mental health contact

    •	employment status

    •	school enrollment

    •	offence category

The dataset is intentionally small and simplified for demonstration purposes.


## METHODOLOGY

The project follows a standard machine learning workflow:

### 1. Data Preparation

       •	dataset loaded and cleaned

       •	categorical variables encoded

       •	no missing values

### 2. Train/Test Split

       •	80% training data

       •	20% test data

### 3. Model Selection

       Logistic Regression was chosen because it is:

       •	interpretable

       •	auditable

       •	appropriate for policy environments

       •	easier to explain to non-technical stakeholders

### 4. Model Evaluation

       Model performance evaluated using:

      •	Accuracy

      •	ROC AUC

      •	Precision / Recall

      •	F1 Score


## MODEL PERFORMANCE

       Metric	Score

       Accuracy	0.57

       ROC AUC	0.76

       F1 Score	0.62

       Average Precision	0.64

Given the small dataset (70 records), the model shows meaningful discriminatory ability.

An AUC of 0.76 indicates that in 76% of cases the model ranks a youth who reoffends higher than one who does not.
Model performance would likely improve significantly with larger operational datasets.


## KEY RISK FACTORS IDENTIFIED

       Strongest predictors of reoffending:

         •	Prior violent offence

         •	Violent offence category

         •	Prior mental health contact

      Protective factors identified:

         •	Employment status

         •	School enrollment

         •	Prior drug offence history (possible intervention effect)

These findings align with existing research in Youth justice.


## REPOSITORY STRUCTURE

      Project-Release
      │
      ├── New_Updated_Project.ipynb
      ├── dataset.csv
      └── README.md
