# HR Employee Retention Analysis & Prediction

📝 Project Overview
This project focuses on a crucial aspect of Human Resources (HR) management: Employee Retention.   

 By analyzing a dataset of current and past employees. 

<p>the goal is to identify key factors that influence an employee' decision to leave<br> the company
and to build a predictive model to forecast future attrition.</p>

 <h3>The analysis follows a structured approach:</h3>

- Exploratory Data Analysis (EDA)

- Data Visualization 

- Model Building (Logistic Regression) 

- Accuracy Measurement.

<h3>Key Objectives</h3>

- Identify variables (e.g., salary, department, work-life balance)<br> that have the most significant impact on employee turnover.

- Visualize the correlation between key features and the retention rate.

- Develop a Logistic Regression model to predict if an employee will leave the company.

- Measure and evaluate the model's accuracy.

<h3>⚙️ Setup and Installation</h3> 

- To run this project locally, you will need a Python environment with the following libraries installed.

<h3>Prerequisites</h3>
  - Python 3.x<br>  
  - Jupyter Notebook (or an IDE like VS Code, Spyder)

<h3>Installation</h3>
  Clone the repository and install the required packages using pip:

  ```
    git clone https://github.com/your-username/hr-retention-analysis.git 
    cd hr-retention-analysis
    pip install pandas numpy matplotlib seaborn scikit-learn
 ```

<h3>Files in this Repository</h3>

hr_analysis_.ipynb: The main Jupyter Notebook containing all the data cleaning, EDA, visualizations,<br> model training, and evaluation steps.

[HR_comma_sep.csv](HR_comma_sep.csv): The raw dataset used for the analysis (please ensure this file is<br> included or link to its source).

<h3>🖼️ Key Visualizations</h3>
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

<h3>🧠 Model Building and Results</h3>

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

<p>This accuracy provides a strong foundation for an early warning system that HR can use to identify<br> employees at risk of leaving and intervene proactively.</p>


