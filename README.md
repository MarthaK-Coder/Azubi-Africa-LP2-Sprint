# PREDICTING CUSTOMER CHURN FOR VODAFONE USING CLASSIFICATION MODEL
## PREDICTING CUSTOMER CHURN FOR VODAFONE USING CLASSIFICATION MODEL <a name="PREDICTING CUSTOMER CHURN FOR VODAFONE USING CLASSIFICATION MODEL"></a>

<div align="right">
  <img src="635_vodafone.png" alt="Image" width="200" height="200">
</div>
This is repository containing a summary of project done in LP2 Azubi Sprint

# Brief Project Description
The Churn Analysis using Classification Model project aims to predict customer churn, a critical business metric, by employing classification algorithms on a dataset containing customer information. Customer churn, the phenomenon where customers stop using a service, can have significant financial implications for businesses. This project utilizes machine learning techniques to proactively identify customers at risk of churning,enabling targeted retention strategies and improved customer satisfaction.

In this project we using the CRISP -DM Frame work to guide in our analysis

# Table of Contents
- [BusinessUnderstanding](#Business Understanding)
- [DataPreparation](#Data Preparation)
- [Modelling](#Modelling)
- [Evaluation](#Evaluation)
- [ConclusionandInsights](#Data Preparation)
## Business Understanding <a name="Business Understanding"></a>
The objective of this project is to help a Vodafone telecommunications company use classification models to gain insight into their customer data, determine the lifetime value of each customer, pinpoint the major variables affecting customer churn rates, and create predictive models to ascertain whether a customer will leave or not.
The stakeholders in this project are : 
- Management Team,
- Marketing Department
- Customer Service representatives,
- Data Analysts and Data Scientists, 
- Product Development, Sales Team, Operations Team,
- Legal and Regulatory Affairs ensuring that any decisions made based on the churn analysis comply with legal and regulatory requirements
- Finance Team: Stakeholders in the finance department who want to understand the financial implications of churn and the cost-effectiveness of retention strategies.
- Investors and Shareholders: Individuals or groups who have invested in Vodafone and are interested in the company's performance and strategies to address churn.
- End Users (Customers): The customers themselves are important stakeholders. Understanding their reasons for churning can provide valuable insights for improvement.
## Data Preparation <a name="Data Preparation"></a>
The data preparation step is a crucial phase that lays the groundwork for effective analysis and modeling. In this phase, we focused on collecting, assessing, and enhancing the raw data to ensure its quality and suitability for further analysis.

Data Collection from Azubi Database
We initiated the data collection process by interfacing with the Azubi Database using Python. By leveraging Python's database connectivity tools, we extracted the relevant data sets required for our churn analysis project. This enabled us to ensure that we had access to the most accurate and up-to-date information directly from the source.

Reading Excel and CSV Files
In addition to the Azubi Database data, we integrated supplementary information by reading Excel and CSV files. These files contained valuable details about customer attributes, transaction histories, and related factors. By employing Python's data manipulation libraries, we imported and harmonized these external data sources, ensuring a comprehensive and enriched dataset.

Answering Smart Questions - Exploratory Data Analysis (EDA) and Hypothesis Testing
The data preparation phase also involved exploring the data to uncover insights and answer relevant questions. Through Exploratory Data Analysis (EDA), we delved into the dataset's characteristics, distributions, correlations, and potential patterns. This helped us understand the data's underlying structure and identify initial trends.

Additionally, we formulated and tested hypotheses based on our domain knowledge and business objectives. Hypothesis testing allowed us to validate assumptions and uncover relationships between variables that could be significant for churn analysis.

By addressing smart questions during this phase, we not only gained a better understanding of the data but also paved the way for focused analysis in subsequent stages.

Overall, the data preparation step played a vital role in curating a high-quality dataset and initiating insightful analyses. Through data collection, integration, and exploratory techniques, we ensured that our subsequent analysis and modeling efforts would be well-informed and effective in addressing the project's objectives.
## Modelling <a name="Modelling"></a>
The modeling phase involves building, training, and evaluating various classification models to identify the best-performing model for our churn analysis project. In this phase, we followed a structured approach to ensure that we select the most accurate and effective model.

**Data Splitting and Balancing**
We began by splitting the dataset into training and testing sets. This separation allowed us to assess the model's performance on unseen data, providing a realistic measure of its effectiveness.

To address class imbalance, we employed techniques such as oversampling or undersampling to create a balanced training dataset. This ensured that the model was trained on representative samples from both churn and non-churn classes.

**Initial Model Creation and Evaluation**
We then proceeded to create, train, and evaluate several classification models, including:

Logistic Regression
Random Forest Classifier (RFC)
Support Vector Machine (SVM)
K-Nearest Neighbors (KNN)
Linear Discriminant Analysis (LDA)
Quadratic Discriminant Analysis (QDA)
We evaluated these models using the accuracy score as a performance metric. Based on the initial evaluation, we identified the Random Forest Classifier (RFC) as the best-performing model.

**Advanced Model Training with Hyperparameter Tuning**
With the RFC identified as the most promising model, we performed advanced model training by tuning its hyperparameters. This involved using GridSearchCV to systematically explore different hyperparameter combinations and identify the optimal settings.

After hyperparameter tuning, we once again compared the performance of the six models using the accuracy score. This step allowed us to gauge the improvements achieved through hyperparameter tuning and determine the final best-performing model.

**Model Selection and Conclusion**
After completing the hyperparameter tuning process, we observed an improvement in the accuracy score, with the RFC model consistently outperforming the other models. Therefore, we concluded that the Random Forest Classifier (RFC) was the optimal choice for our churn analysis project.

The modeling phase was pivotal in identifying the most accurate and reliable model for predicting customer churn. By systematically evaluating various models and refining their performance through hyperparameter tuning, we ensured that our chosen model would provide robust and actionable insights for addressing the project's objectives.

## Evaluation <a name="Evaluation"></a>
The evaluation phase involves assessing the performance of our chosen model and deriving insights from its predictions. In this phase, we focused on predicting churn on the X-test set using the best estimator (Random Forest Classifier) obtained from the modeling phase.

**Predictions and Churn Rate Calculation**
We used the best-performing model, the Random Forest Classifier (RFC), to predict churn on the X-test set. By applying the model to the unseen data, we generated predictions that allowed us to classify customers into churn and non-churn categories. From these predictions, we calculated the churn rate by determining the proportion of customers predicted as churned out of the total.

**Churn Rate Analysis**
Analyzing the churn rate distribution from the model's predictions provided valuable insights. Notably, we observed that the "no churn" rate had the highest percentage among the total outcomes. This observation suggests that the dataset's features contribute to the model's prediction of non-churn cases.

**Feature Importance Analysis**
To delve deeper into the factors influencing the churn rate, we conducted a feature importance analysis. This analysis involved ranking the features based on their impact on the churn rate. The results highlighted the following features as having the largest impact on predicting churn rate:

Contract_Month-to-month
Tenure
TotalCharges
MonthlyCharges
ChargesperYear
These findings offer valuable insights into the attributes that play a crucial role in predicting customer churn. By understanding which features contribute the most to churn predictions, businesses can tailor their strategies to effectively address churn-related concerns.

The evaluation phase allowed us to assess the model's performance, understand the distribution of predicted outcomes, and identify the key features influencing churn rate predictions. These insights serve as a foundation for making informed decisions to enhance customer retention strategies and mitigate churn risks.

Before Deployment we need to go back to the datasets and explore models once again.

## Conclusion and Insights <a name="Conclusion and Insights"></a>
In conclusion, the comprehensive churn analysis conducted for Vodafone offers profound insights that can reshape the company's customer retention strategies. The identification of prominent features, including contract type, tenure, total charges, monthly charges, and charges per year, illuminates the critical factors influencing customer churn. This information is pivotal for Vodafone to recalibrate its approach towards customer engagement and satisfaction. By strategically focusing on retaining customers through tailored communication strategies, Vodafone can harness the potential of personalized messages that resonate with varying customer segments. The recommendation to continuously monitor customer behavior aligns with the dynamic nature of the telecommunications industry, ensuring that churn mitigation strategies remain effective in the face of evolving trends. Ultimately, the analysis underscores the power of data-driven decision-making, providing a solid foundation for Vodafone to proactively address churn risks and cultivate a more engaging and lasting customer relationship.

