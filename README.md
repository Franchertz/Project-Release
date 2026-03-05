**Youth Justice Risk Prediction Prototype**

**Early Risk Identification for Youth Justice Services**
________________________________________
**Project Overview**

This project demonstrates how machine learning can support evidence-informed decision-making in youth justice services.
The prototype model estimates the likelihood of youth reoffending within two years, using a small structured dataset representing youth justice case characteristics.
The objective is not to replace professional judgment, but to provide staff with an additional decision-support lens when prioritising interventions and allocating limited program resources.
This project was developed as a portfolio demonstration of applied data science in a youth justice context.
________________________________________
**Policy & Operational Motivation**

Youth justice systems must allocate limited resources (mental health services, employment support, supervision intensity) to youth most in need.
However, frontline staff often must make these decisions without structured analytical support.
This prototype explores how interpretable machine learning models can help:
•	identify higher-risk youth earlier
•	prioritise interventions
•	support case planning decisions
•	inform program allocation
The approach emphasizes transparency and interpretability, which are critical in justice environments.
________________________________________
**Dataset**

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
________________________________________
**Methodology**

The project follows a standard machine learning workflow:

1. Data Preparation

•	dataset loaded and cleaned
•	categorical variables encoded
•	no missing values

2. Train/Test Split

•	80% training data
•	20% test data

3. Model Selection

Logistic Regression was chosen because it is:

•	interpretable
•	auditable
•	appropriate for policy environments
•	easier to explain to non-technical stakeholders

4. Model Evaluation

Model performance evaluated using:

•	Accuracy
•	ROC AUC
•	Precision / Recall
•	F1 Score
________________________________________
**Model Performance**

Metric	Score
Accuracy	0.57
ROC AUC	0.76
F1 Score	0.62
Average Precision	0.64

Given the small dataset (70 records), the model shows meaningful discriminatory ability.
An AUC of 0.76 indicates that in 76% of cases the model ranks a youth who reoffends higher than one who does not.
Model performance would likely improve significantly with larger operational datasets.
________________________________________
**Key Risk Factors Identified**

Strongest predictors of reoffending:

•	Prior violent offence
•	Violent offence category
•	Prior mental health contact

Protective factors identified:

•	Employment status
•	School enrollment
•	Prior drug offence history (possible intervention effect)
These findings align with existing research in youth justice.
________________________________________
**Ethical Considerations**

Predictive models in justice systems must be applied carefully.

Important safeguards include:
•	fairness and bias testing
•	transparency of model logic
•	human oversight in all decisions
•	use as decision-support, not automation

This prototype emphasizes interpretability and responsible AI principles.
________________________________________
**Repository Structure**

Project-Release
│
├── New_Updated_Project.ipynb
├── dataset.csv
└── README.md
________________________________________
**Important Note**

This project is a demonstration prototype for learning and discussion purposes only and is not intended for operational use without extensive validation and ethical review.
________________________________________
