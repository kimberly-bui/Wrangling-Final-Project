# BAIS:3250 Data Wrangling

## Kim Bui & Camille Eastvold  

### COVID-19 and Factors Relating to Healthcare Attrition 

This project investigated the impact of COVID-19 on healthcare worker attrition using Jupyter Notebooks for data analysis. We analyzed data from two publicly available sources: a 2018 National Sample Survey of Registered Nurses and a 2022 Healthcare Employee Attrition dataset.

**Data Acquisition and Preparation**

1. **Downloaded** the 2022 Healthcare Employee Attrition dataset (watson_healthcare_modified.csv) from Kaggle.
2. **Cleaned and transformed** the data using Jupyter Notebooks, including handling missing values, converting data types, and creating new features.
3. **Web-scraped** data from the 2018 National Sample Survey of Registered Nurses.
4. **Cleaned and transformed** the web-scraped data, ensuring consistency with the 2022 dataset.
5. **Merged** the two datasets based on relevant variables.

**Data Analysis and Modeling**

1. **Exploratory Data Analysis (EDA):** Conducted EDA to understand data distributions, correlations, and potential relationships between variables.
2. **Hypothesis Testing:** Used statistical tests to determine the significance of differences in job satisfaction, overtime hours, and income between pre- and post-pandemic periods.
3. **Correlation Analysis:** Explored the correlation between income and attrition using Pearson Correlation Coefficient.
4. **Regression Modeling:** Utilized linear regression to identify factors contributing to high attrition rates.

**Key Findings**

* **Job satisfaction** significantly decreased post-pandemic due to increased workload, stress, and staffing shortages. 
* Income showed a **weak correlation** with job satisfaction, suggesting other factors like work-life balance are more important.
* **Overtime hours** increased in 2022 compared to 2018, potentially due to burnout or staffing issues.

**Conclusion**

These findings suggest the need for healthcare institutions to prioritize employee well-being, fair compensation, and effective workload management to improve retention. Further research with targeted datasets and qualitative studies could provide deeper insights.

**Technical Implementation**

The entire analysis was conducted using Jupyter Notebooks, executing the notebooks in the following order:

1. **00_webscrape.ipynb:** Web-scraped data from the 2018 National Sample Survey.
2. **01_kaggle.ipynb:** Cleaned and transformed the 2022 Healthcare Employee Attrition dataset.
3. **02_merge.ipynb:** Merged the two datasets.
4. **03_analysis.ipynb:** Performed exploratory data analysis, hypothesis testing, correlation analysis, and regression modeling. 

This project demonstrates the effective use of Jupyter Notebooks for data wrangling, analysis, and modeling in a real-world healthcare scenario.
---

## Data source
- https://www.kaggle.com/datasets/jpmiller/employee-attrition-for-healthcare?resource=download
 
- https://pmc.ncbi.nlm.nih.gov/articles/PMC10742910/#healthcare-11-03173-t001 
 




---
