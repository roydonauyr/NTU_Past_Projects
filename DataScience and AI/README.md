# 1. BC2406 Data Analytics
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/roydonauyr/-Analytics-Renewable-Energy-impacts-GDP
)
![GitHub repo size](https://img.shields.io/github/repo-size/roydonauyr/-Analytics-Renewable-Energy-impacts-GDP
)
![GitHub language count](https://img.shields.io/github/languages/count/roydonauyr/-Analytics-Renewable-Energy-impacts-GDP
)
![GitHub last commit](https://img.shields.io/github/last-commit/roydonauyr/-Analytics-Renewable-Energy-impacts-GDP
)

**A project on how the renewable energy could be useful in predicting/improving GDP and growth**

# Executive summary
Studies on Environmental Factors:
This report studies environmental factors, primarily renewable energy, and their relationship with two variables – GDP per capita, and GDP per capita growth, over a period of 28 years (1991 to 2018). Due to the presence of many strong outliers for GDP per capita growth, the relationship was studied by converting it into a categorical variable (Acceptable growth).

Linear Regression and Continuous CART Model (GDP per capita):
The study was conducted using Linear regression and continuous CART models. We tested different models and explored how the results varied across different datasets (Splitting by economy type). Upon many comparisons, we have found that continuous CART was the better model of the two for all datasets (Lower RMSE). Using CART, the results are shown below:
Renewable Energy Consumption and Population Growth are found to be the two most significant variables for predicting GDP per capita for all datasets. Moreover, environmental variables generally have high importance with CO2 emissions being top 4. It was also observed that CO2 emissions had a negative weight for developed countries
Upon further studying the variable importance of Renewable electricity output and Renewable energy consumption over three time periods (1991-1999, 2000-2008, 2009-2018) we observed:
Overall dataset: Renewable electricity output’s importance increased over the years.
Developed Countries dataset: Renewable energy consumption’s importance increased 
Developing Countries dataset: Both variables’ importance remained constant.
Hence, Renewable energy consumption is a strong predictor for the GDP per capita of a country, and its importance in the developed countries model will likely increase over time.

Logistic Regression, Categorical CART Model (Acceptable growth):
The study was conducted using Logistic regression and categorical CART models. Just like above, we compared the models and found that CART has a better prediction accuracy for all datasets except for developing countries. Using CART and logistic models, the results are:

CART:
In general, environmental variables are strong predictors of Acceptable growth for all datasets with CO2 emissions being a relatively strong predictor.
Overall dataset: Population total and nitrous oxide emissions are the two most significant variables. Moreover, both renewable energy variables are good predictors.
Developed Countries dataset: Population total and CO2 emissions are the two most significant variables. 
Just like above, we studied the trend of the two renewable variables over three time periods:
Overall dataset: Renewable electricity output’s variable importance increases over time.
Developed Countries dataset: Renewable energy consumption’s importance increased over time.
Logistic Regression (Developing countries dataset): 
CO2 emissions and greenhouse gases are good predictors of Acceptable growth. Other environmental variables are also close to statistical significance. Moreover, Renewable energy consumption’s variable importance and strength as a predictor increases over time.
Hence, from the two models, we can conclude that both renewable energy variables are strong predictors for Acceptable growth for the overall dataset model. Moreover, renewable energy 
consumption’s strength as a predictor increases over time.


# Appendix:
## Some EDA:
![image](https://user-images.githubusercontent.com/44868878/178106155-c437fe3b-03e3-468c-8f7b-4288b28b3d6e.png)
![image](https://user-images.githubusercontent.com/44868878/178106164-de27bd22-67ec-445e-9828-4a43ceacdd79.png)

## Model Diagnostics:
![image](https://user-images.githubusercontent.com/44868878/178106173-cc01ef50-ce53-4aac-ad5b-f22be05ed651.png)
![image](https://user-images.githubusercontent.com/44868878/178106176-f30fb9de-02c6-4210-9cad-f8105bbd1a83.png)

## CART Pruned tree
![image](https://user-images.githubusercontent.com/44868878/178106191-b83c2971-747b-4ba4-a0ac-b8bcd60c65b0.png)

**FULL REPORT CAN BE FOUND IN PDF**

# 2. BC2407  Advanced Data Analytics 
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/roydonauyr/PROJECT-BC2407-Advanced-Analytics
)
![GitHub repo size](https://img.shields.io/github/repo-size/roydonauyr/PROJECT-BC2407-Advanced-Analytics
)
![GitHub language count](https://img.shields.io/github/languages/count/roydonauyr/PROJECT-BC2407-Advanced-Analytics
)
![GitHub last commit](https://img.shields.io/github/last-commit/roydonauyr/PROJECT-BC2407-Advanced-Analytics
)

Hello! We are Sem 3 Team 2 taught by Prof Eric Kwon! Our Project Title is Carity, and we hope to use analytics to bring clarity to Healthcare in Africa!

Files:
- Project Report
- Presenation Slides
- Jupyter Notebook w/ Model Preparation and Machine Learning Code
- Datasets were too large and could not be uploaded :(
  - https://www.kaggle.com/nehaprabhavalkar/av-healthcare-analytics-ii
  - https://health.data.ny.gov/Health/Hospital-Inpatient-Discharges-SPARCS-De-Identified/82xm-y6g8


## So what is the problem?

**The Business Problem** lies in inaccurate assessment of Length of Stay (LOS) in South African Hospitals.

Doctors are at the forefront of a hospital's operations, yet their scope of decisions arguably fail to include the wide range of administrative constraints faced by the hospital in its entirety. This leads to even wider implications like Patient Health Risks, Poor Patient Experience, Higher Healthcare Charges, Operational Delay and Inefficiency, and Increased Financial Burden on the hospital.

HealthMan is a privately owned healthcare consultancy specialising in the management and administration of hospitals in South Africa. Their mission is to promote the professional and commercial interests of hospitals. To solve the above problem, we as interns at HealthMan have come up with a two-pronged approach using Analytics at its core.

## Overview of Business Problem and Approach
![image](https://user-images.githubusercontent.com/64303732/161944087-5a49e1fd-0f6d-4f91-927a-13b1da2dca8a.png)

## Target Outcome 1 - Consistent and Accurate Presciption of LOS

This approach uses **Machine Learning** Models to help doctors predict LOS by providing a benchmark value based on a wide range of hospital data.

The models trialled were **Multi-Adaptive Regression Splines (MARS), Classification and Regression Tree (CART), and Random Forest**. For more details, please refer to our Python Notebook!

Based on the most **accurate, explainable, and easy to implement** model, we embed our predictions in a Hospital's EMR System for doctors to refer to in real-time during consultations.

Lastly, the **Integrated Hospital Management Dashboard** serves to supplement doctor's decisions by providing a non-technical, high-level overview of the hospital situation.

## Target Outcome 2 - Targeting Unnecessary LOS

To further help hospitals customise a solution for improving LOS, we use Variable Importance to identify the most significant factors influencing LOS. Feature Importance can be generated from CART and Random Forest. This data is then taken in by our Interactive Dashboard and transformed into visually-appealing data stories.


## Overview of Solution
![image](https://user-images.githubusercontent.com/64303732/161944213-8f964249-577b-4310-bccc-05bab1f80c01.png)

## Tableau Dashboards
### Hospital Dashboard
![image](https://user-images.githubusercontent.com/64303732/161944419-41f1c1de-43e3-4f3b-b7ea-b4ddca972e66.png) 
### Patient Dashboard
![image](https://user-images.githubusercontent.com/64303732/161944439-c06fea0f-9487-49fc-a423-e70314de08d6.png)

# 3. CZ3005 AI Project

![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/roydonauyr/AI_CZ3005_Project1
)
![GitHub repo size](https://img.shields.io/github/repo-size/roydonauyr/AI_CZ3005_Project1
)
![GitHub language count](https://img.shields.io/github/languages/count/roydonauyr/AI_CZ3005_Project1
)
![GitHub last commit](https://img.shields.io/github/last-commit/roydonauyr/AI_CZ3005_Project1
)

Search Algorithms

To RUN: cd AI_CZ3005_Project1-main python main.py
