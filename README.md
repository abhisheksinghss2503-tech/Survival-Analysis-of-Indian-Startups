🚀 Survival Analysis of Indian Startups

📌 Project Overview

This project analyzes the survival patterns of Indian startups founded after the year 2000 using classical statistical survival analysis techniques and modern machine learning approaches. The objective is to identify factors influencing startup longevity and compare the predictive performance of traditional and non-parametric survival models.

The study applies:

Kaplan-Meier Survival Analysis
Log-Rank Statistical Tests
Cox Proportional Hazards Model
Random Survival Forest (RSF)

The dataset consists of Indian startups with information about founding year, funding rounds, funding amount, market sector, city, and operational status. The project investigates how these factors impact startup survival and failure risk.

🎯 Objectives

Estimate startup survival probabilities using Kaplan-Meier curves.
Compare survival distributions across sectors and cities.
Evaluate statistical significance using Log-Rank tests.
Quantify covariate effects using Cox Proportional Hazards regression.
Capture complex non-linear relationships using Random Survival Forest.
Compare model performance using Concordance Index (C-Index).

📊 Dataset Information

The original dataset contains information on Indian startups, including:

Company Name
Market Sector
City
Founded Year
Funding Rounds
Total Funding (USD)
First Funding Date
Last Funding Date
Operational Status
Data Cleaning Steps
Removed startups founded before 2000.
Handled missing values.
Removed invalid observations.
Created survival time and event indicators.
Processed date variables for survival analysis.

Final analytical dataset:

756 startups
57 observed events (Closed/Acquired)
699+ censored observations
🛠 Technologies Used
Programming Language
Python
Libraries
pandas
numpy
matplotlib
seaborn
lifelines
scikit-survival
scikit-learn
statsmodels
Statistical Methods
Survival Analysis
Kaplan-Meier Estimation
Log-Rank Test
Cox Proportional Hazards Regression
Random Survival Forest
Multicollinearity Analysis (VIF)
Residual Diagnostics

🔍 Methodology

1. Exploratory Data Analysis (EDA)
Startup founding trends
Startup status distribution
Top startup cities
Top startup sectors
Survival year distribution
Correlation analysis

3. Kaplan-Meier Survival Analysis

Estimated startup survival probabilities over time and compared survival across:

Market sectors
Funding categories
Startup cities

3. Log-Rank Testing

Performed statistical tests to determine whether survival differences across groups were significant.

4. Cox Proportional Hazards Model

Used to estimate hazard ratios and understand the effect of:

Funding rounds
Total funding
Founding year
Market sector
City

5. Random Survival Forest

Implemented a machine learning survival model capable of capturing:

Non-linear relationships
Complex interactions
High-dimensional survival patterns

📈 Key Findings

Kaplan-Meier Analysis
Most Indian startups exhibit high survival probabilities.
Sector and city-level differences exist in startup survival patterns.
Log-Rank Tests
Market sector significantly affects startup survival.
City-level differences are statistically significant.
Funding categories show weaker significance.
Cox Proportional Hazards Model
Funding variables showed limited direct impact on survival.
Education and Software sectors demonstrated relatively better survival.
Bengaluru and Mumbai startups showed comparatively favorable outcomes.
Random Survival Forest
Captured complex relationships missed by Cox regression.
Achieved superior predictive performance.

📊 Model Performance

Model	Concordance Index (C-Index)
Cox Proportional Hazards	0.715
Random Survival Forest	0.815

The Random Survival Forest outperformed the Cox model, indicating that non-linear relationships play an important role in startup survival prediction.

📁 Project Structure

Survival-Analysis-Indian-Startups/
│
├── data/
│   └── Indian_Startups_Dataset.csv
│
├── notebooks/
│   └── Startup_Survival_Analysis.ipynb
│
├── images/
│   ├── KM_Curves.png
│   ├── LogRank_Results.png
│   ├── Cox_Model.png
│   └── RSF_Results.png
│
├── report/
│   └── MSc_Research_Project.pdf
│
├── requirements.txt
│
└── README.md


👨‍💻 Author

Abhishek Singh

M.Sc. Statistics
Banaras Hindu University (BHU)
