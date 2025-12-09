# Data Science Portfolio

**More detailed README files are included inside the individual project.**

### Main Components Being Analyzed
- A collection of data science projects demonstrating skills in statistical analysis, machine learning, network analysis, clustering, and predictive modeling.
Each project includes clear objectives, methodology, results, and code improvements, with links to full detailed documentation.

## Table of Contents
- Board of Directors Network Analysis
- Prediction of International Education Cost
- Statistical Analysis for Investment Prediction

## 1. Board of Directors Network Analysis

### Overview
- Analyzes corporate board networks using director and company data to reveal relationships, influence patterns, and board dynamics. Uses network analysis, demographic insights, and temporal trends to identify key players and structural patterns.

### Main Components Being Analyzed
        1. Director Information:
           - Names
           - Software backgrounds (boolean t/f)
           - Start/End dates
           - Company associations
        2. Network Analysis:
           - Bipartite networks (directors-companies)
           - Centrality measures
           - Connected components
           
### Highlights
- Built from SEC DEF 14A filings (U.S. public company data)
- Bipartite networks linking directors and companies
- Network Metrics:
           - Eigenvector centrality
           - Degree centrality
           - Betweenness centrality
- Temporal Analysis:
           - Director tenure lengths
           - Board turnover rates
           - Appointment patterns
- Director Demographics:
           - Age distribution
           - Compensation patterns
           - Software background distributio

### Technologies
- Python 3.11+, Jupyter Notebook
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- networkx

### Detailed README:
- DATA-PROJECTS/Analyzing corporate board relationships and director networks using a dataset/README.md

## 2. Prediction of International Education Cost

### Overview
- Predicts the total cost of studying abroad for international students by analyzing tuition, rent, living costs, visa, and insurance expenses. Compares regression models, applies clustering, and visualizes affordability patterns.

### Dataset Content
        Main cost components being analyzed:
        - Tuition fees (USD)
        - Living costs
        - Rent costs
        - Visa fees
        - Insurance costs
        - Exchange rates
        
### Key Steps
- Data Preparation – Handle missing values, feature engineering (Living_Cost_Total, Rent_Total, Total_Cost), scaling
- Modeling – Linear Regression, Polynomial Regression, Decision Tree (tuned max_depth)
- Clustering – KMeans on top cost drivers; affordability grouping
- Custom Tool – University lookup for predicted cost and affordability cluster

### Project Objectives
        1. Analyze cost variations across:
           - Different countries
           - Program levels
           - Universities
        2. Identify:
           - Most/least affordable study destinations
           - Cost clustering patterns
           - Total cost predictions
        3. Help students make informed decisions about:
           - Financial planning
           - Destination selection
           - Program choices
          - Statistical modeling libraries

### Results
Model	R² Score	RMSE ($)	MAE ($)
Linear Regression	1.0000	0.00	0.00
Polynomial Regression	1.0000	0.00	0.00
Decision Tree (Tuned)	0.9919	3,603.92	2,369.87

### Technologies
- Python 3.11+, Jupyter Notebook
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

### Detailed README:
- DATA-PROJECTS/International education costs/README.md

## 3. Statistical Analysis for Investment Prediction

### Overview
- Performs statistical investigation to support investment prediction, combining distribution analysis with regression modeling. Includes data exploration, classical and robust regression techniques, and visualization of statistical patterns.

### Key Features
- Data ingestion & inspection
- Visualization of payroll/investment trends
- Outlier detection & discussion
- Linear Regression models (OLS & Huber Regressor)
- Distribution experiments (Central Limit Theorem)
- Model evaluation with MAE & MSE
- Log transformation on revenue data for improved prediction
- Logistic regression for negative media coverage classification

### Data Analysis Components
        1. Dataset Characteristics:
          - Time series data spanning 24 months
          - Key variables include Payroll, Revenue, and Media Coverage
          - Base 10 log transformation of Revenue included
        2. Model Types:
          - Linear regression (including OLS and Huber Regressor)
          - Log transformation analysis
          - Revenue prediction modeling
        3. Key Features:
          - Monthly progression metrics
          - Financial indicators (Payroll, Revenue)
          - Media sentiment tracking

### Technologies
- Python 3.8+, Jupyter Notebook
- pandas, numpy
- seaborn, matplotlib
- scikit-learn

### Detailed README:
- DATA-PROJECTS/Statistical analysis for investment prediction/README.md

**Data Analysis: pandas, numpy**

**Visualization: matplotlib, seaborn, plotly**

**Modeling: scikit-learn**

**Graph Analysis: networkx**

**Notebooks: Jupyter**
  
### 4. Contributing
- Each project lives in its own folder with a self-contained README.

Contact:

Kundan Singh Shekhawat

📧 kundansingh.shekhawat@students.mq.edu.au

🔗 GitHub (https://github.com/kundansingh012/DATA-PROJECTS)

