# Lead Scoring Case Study: Conversion Optimization

## Project Overview
This project focuses on building a predictive model for **X Education**, an online course provider, to identify "Hot Leads". With a typical lead conversion rate of approximately 30%, the company required a system to assign a lead score (0-100) to each prospect. This allows the sales team to prioritize high-potential leads and target a CEO-mandated conversion rate of 80%.

---

## Technical Methodology
The project follows a standard data science pipeline:
* **Model Type:** Logistic Regression.
* **Data Preparation:** Handled missing values (specifically the 'Select' level in categorical fields), created dummy variables, and performed feature scaling.
* **Feature Selection:** Utilized **Recursive Feature Elimination (RFE)**, VIF, and p-values to refine the model.
* **Evaluation Metrics:** The model was evaluated using Accuracy, Sensitivity, Specificity, and the ROC curve.

---

## Key Findings & Observations

### Model Performance
The model demonstrated consistent results across both training and testing datasets:
* **Accuracy:** ~80% 
* **Sensitivity:** ~77% 
* **Specificity:** ~80% 
* **Lead Score Threshold:** A conversion probability higher than **42%** is identified as the optimal tradeoff between Precision and Recall to classify a "Hot Lead".

### Critical Features
The final model identifies the following as the most influential features for conversion[cite: 321]:
* **Total Time Spent on Website:** A primary indicator of interest[cite: 326, 336].
* **Lead Source:** Leads from **Google** and **Direct Traffic** are most frequent, while **Welingak Website** and **Reference** show the highest conversion ratios[cite: 325, 334, 335].
* **Occupation:** While most leads are currently unemployed, **Working Professionals** have the highest conversion rate[cite: 328, 337].
* **Engagement:** "SMS Sent" as the last activity correlates with the highest conversion rate[cite: 337].

---

## Business Recommendations
* **Prioritize Engagement Channels:** Focus sales efforts on leads whose last activity was receiving an SMS or opening an email[cite: 214, 337].
* **Focus on Specific Origins:** Concentrate resources on leads originating from **API** and **Landing Page Submissions**, as they represent the bulk of conversions[cite: 331, 333].
* **Target Professional Demographics:** Tailor marketing content for working professionals to capitalize on their high conversion potential[cite: 328, 337].
