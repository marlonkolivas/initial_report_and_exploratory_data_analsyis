# Required Capstone Assignment 20.1: Initial Report and Exploratory Data Analysis (EDA)
In this module, you will work on performing exploratory data analysis (EDA) to develop an initial report for your capstone project. You will use EDA to see what data can reveal beyond the formal modeling, hypothesis testing task, and data training to provide a better understanding of dataset variables and the relationships between them. You are encouraged to spend your time in this module cleaning your data and use feature engineering and EDA techniques to create visualizations to make sense of your findings. Additionally, you will also be required to use one of the ML algorithms you have learned so far in the program to develop a baseline model to use as a comparison in Module 24. You will have time in Module 24 to include additional models, clean the code, and make your work presentable for technical and non-technical audiences. For now, you will do the ‘heavy lifting’ of finding the answer to your research question.

Note: 
I have revised the question that I have intended to answer. Below is the new question: <br>
**How can machine learning be used to predict salaries and recommend optimal AI job roles for professionals in the global AI job market?**

1. The research question you intend to answer (in one sentence, if possible)<br>
How can machine learning be used to predict salaries and recommend optimal AI job roles for professionals based on their skills, experience, and location in the global AI job market?

2. Your expected data source(s) (as either a link to existing data or a sentence describing where you will source the data from): <br>
**[Global AI Job Market & Salary Trends 2025](https://www.kaggle.com/datasets/bismasajjad/global-ai-job-market-and-salary-trends-2025)**


3. The techniques you expect to use in your analysis:<br>
Data Cleaning and Data Processing<br>
Exploratory Data Analysis<br>
Feature Engineering<br>
Train/Test Split<br>
Preprocessing and Random Forest Regressor Baseline Model Pipeline<br>
Cross Validation<br>
Model Evaluation (MAE, RMSE, $R^2$) Metrics<br>

Regression Analysis (for Salary Prediction)
I will use supervised regression models to predict continuous salary values based on multiple independent variables (such as experience, education, country, and skill set).<br>
Classification Techniques (for Job Role Recommendation)
I will apply multi-class classification algorithms to assign a candidate to the most suitable AI role category (e.g., Data Scientist, ML Engineer, NLP Specialist) based on input features.

5. The expected results<br>
The project will yield a functional prototype or dashboard where users can input their profile (skills, education, experience, location) and receive both:
- A predicted salary range.
- Recommended AI job roles matching their attributes.<br>
This output will serve as a decision-support tool for job seekers and recruiters alike, enabling data-driven career planning and compensation benchmarking

4. Why this question is important?<br>
This research question is important because it addresses the growing need for data-driven transparency and personalization in the rapidly evolving global AI job market. Traditional methods of assessing salaries and matching candidates to roles are often inconsistent and outdated. By applying machine learning techniques, this study aims to predict fair and competitive salaries while recommending optimal AI job roles based on individual skills, experience, and location.
Such an approach benefits both job seekers and employers, helping professionals make informed career decisions and enabling organizations to align hiring and compensation strategies with real market trends. Academically, the project demonstrates how predictive analytics and recommendation systems can be combined to solve complex, real-world labor market challenges.


## Model Performance
| Metric       | Value   | Interpretation                                                          |
| ------------ | ------- | ----------------------------------------------------------------------- |
| **R² Score** | 0.88    | Model explains 88% of salary variation—a very strong result.            |
| **MAE**      | $15,135 | On average, predictions are within $15k of the actual salary.           |
| **RMSE**     | $21,152 | Occasional larger errors exist, but predictions are generally accurate. |

## R2
The evaluation metrics provide a strong indication that the model performs well in predicting salary outcomes. The R² score of 0.88 shows that the model explains 88% of the variation in salary, which is considered a high level of explanatory power for real-world compensation data.

### MAE
The model’s predictions typically fall within $15k of the true value. Given the wide salary ranges observed across technical roles, particularly in AI and machine learning fields, this level of error is generally acceptable and indicates consistent performance across most predictions.

### RMSE
The RMSE of $21,152 further supports these findings. Since RMSE penalizes larger errors more severely, its higher value suggests that the model occasionally encounters outliers or unusual salary cases where the deviation from the true value is larger.

Overall, the combination of a high R² score, a moderate MAE, and a reasonably controlled RMSE indicates that the model provides reliable and meaningful salary predictions. While it performs strongly as a baseline model, future improvements may include refining feature engineering, addressing outliers, or incorporating additional variables that capture job level or industry-specific characteristics to further reduce error.

## Predicted Versus Actual Plot

<img width="715" height="467" alt="predicted vs actual" src="https://github.com/user-attachments/assets/636929f6-351f-4a19-bb3f-77851ec6d95b" />

