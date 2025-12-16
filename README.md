# HR Retention Analysis & Prediction

##  Project Overview
This project analyzes employee turnover data to identify the key factors driving attrition. Using **Logistic Regression**, I built a model to predict whether an employee will leave the company based on satisfaction levels, salary, and tenure.

**Goal:** Provide actionable insights to HR teams to improve retention rates.

##  Key Insights & Results
* **Retention Rate:** The dataset showed a retention rate of **76.19%**, while **23.81%** of employees left.
* **Salary Impact:** Exploratory Data Analysis (EDA) revealed that employees in the **'low' salary** bracket had the highest churn rate.
* **Model Performance:** The Logistic Regression model achieved an accuracy of **80.16%** on the test dataset.

##  Technologies Used
* **Python 3.9+**
* **Pandas & NumPy:** Data cleaning and manipulation (including numerical encoding of salary categories).
* **Matplotlib & Seaborn:** Visualizing retention impact and salary distributions.
* **Scikit-Learn:** Logistic Regression implementation and model evaluation.

##  Project Structure
├── data/ # Raw HR dataset. <br> 
├── notebooks/ # Jupyter Notebooks for EDA and Modeling. <br>
├── src/ # Python scripts for preprocessing. <br>
├── images/ # Visualizations (Confusion Matrix, Retention Charts). <br>
├── requirements.txt # Python dependencies. <br>
└── README.md.

[HR_comma_sep.csv](HR_comma_sep.csv): The raw dataset used for the analysis (please ensure this file is<br> included or link to its source).

<h3> Key Visualizations</h3>
<p>The visualizations section highlights critical relationships found during the Exploratory Data Analysis (EDA).<br> These charts provide clear insights into which employee characteristics correlate most strongly with the decision to leave the company.</p>

<h3>1. Impact of Salary on Retention</h3>

A bar chart is used to compare the retention rate (Left vs. Stayed) across different salary levels (Low, Medium, High).<br>

 <h3>Insight:</h3><br> 
 - We observed a significantly higher turnover rate among employees with 'Low' salaries, indicating compensation is a major factor in attrition.<br></br>
 <img width="700" height="400" alt="HRImpact of Salary on Employee Retention" src="https://github.com/user-attachments/assets/dd803249-cf4f-45e1-8f6e-a06dc3c19d2f" />

 <h3> 2. Department-wise Retention Correlation.</h3>
   
   - This visualization compares the employee turnover rate across various departments (e.g., Sales, R&D, Technical, Management).

<h3>Insight:</h3> <p>The analysis reveals which departments have a disproportionately high attrition rate,<br> allowing HR to focus retention efforts on specific areas, such as the Technical or Support departments.</p>
<img width="1200" height="500" alt="HRImpact of Department on Employee Retention" src="https://github.com/user-attachments/assets/c1a93b77-c1f6-4617-892e-8331f4a9eeee" />


<h3>- 3. Other Corelations</h3>

Additional plots likely showcase relationships between:

**Satisfaction Level vs. Retention:** To see if dissatisfied employees are the primary drivers of turnover.

**Time Spent at Company vs. Retention:** To identify critical churn points based on tenure.

<h3> Model Building and Results</h3>

<p>Based on the insights gathered from the EDA and visualizations (particularly features like Salary and Department)<br> a Logistic Regression model was built to predict employee retention.</p>

<h3>Model Details</h3>

- <h3>Algorithm</h3>:Logistic Regression (a classification algorithm suited for binary outcomes like 'Left' or 'Stayed').

- <h3>Input Features</h3>:Variables selected based on their statistical significance and clear impact on the target variable.

- <h3>Target Variable:</h3> Left (0 = Stayed, 1 = Left).

### Accuracy

The model's performance was measured on a test set to ensure its predictive capability on unseen data.
```
Metric,Result
Model,Logistic Regression
Accuracy,~80.15%
Interpretation,The model correctly predicts whether an employee will leave or stay approximately 8 out of 10 times.
```

<p>This accuracy provides a strong foundation for an early warning system that HR can use to identify<br> employees at risk of leaving and intervene proactively.</p> <br>

 ## How to Run <br>
 **Clone the repository:**
 ```
    git clone [https://github.com/Miltondevx/hr-analysis.git](https://github.com/Miltondevx/hr-analysis.git)
    cd hr-analysis
    ```

  **Install dependencies:**

    ```
    pip install -r requirements.txt
    ```
 **Run the notebook:**
    ```
    jupyter notebook notebooks/HR_Analysis.ipynb

    ```

## Future Improvements
* Test Random Forest and XGBoost to improve accuracy beyond 80%.
* Deploy the model using Streamlit for a user-friendly HR dashboard.

