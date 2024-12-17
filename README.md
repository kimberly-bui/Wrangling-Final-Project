# COVID-19 and Factors Relating to Healthcare Attrition 

## Kim Bui & Camille Eastvold  

Since 2019, the coronavirus has been infecting the world. Years later the U.S. is still dealing with the symptoms of high turnover and poor retention rates across the healthcare industry. Is the job market still in recovery? 
The COVID-19 pandemic has had profound and lasting effects on the healthcare sector, particularly in the United States. Healthcare institutions continue to grapple with issues such as high turnover, reduced job satisfaction, and an increased workload for remaining staff. Nurses, as a cornerstone of the healthcare workforce, have been disproportionately affected.

This analysis finds trends in job satisfaction, income, and overtime hours by comparing data from 2018 (pre-pandemic) and 2022 (post-pandemic). By identifying key factors contributing to healthcare attrition, this research aims to provide actionable insights for improving retention and addressing burnout among healthcare workers. In this project, we are using 2022 Healthcare Employee Attrition  dataset to find emerging trends after the pandemic to see the changes for nurses using national report data, we obtained from 2018 National Sample Survey of Registered Nurses Nursing Solutions Inc (NSI) .


---

## Data source
- https://www.kaggle.com/datasets/jpmiller/employee-attrition-for-healthcare?resource=download
 
- https://pmc.ncbi.nlm.nih.gov/articles/PMC10742910/#healthcare-11-03173-t001 
 

This project uses two primary sources of data: both are survey results from 2022 Healthcare Employee Attrition dataset from Kaggle and 2018 National Survey for Nursing Solutions Inc. 

2.1 2018 Survey Data

We collected data from the National Sample Survey of Registered Nurses Nursing Solutions Inc, found in the National Library of Medicine. 

The overall findings of the survey were presented in table 3 of this report. Through web scraping script, 00_webscrape.ipynb we were able to gather all contents of the table. The table contained metrics from original 2018 survey data and simulated data calculated by an algorithm. After importing the scraped data into a data frame, we dropped unnecessary columns including the simulated algorithm data. We kept the real survey results in 2018. In the report response data, we gathered results from 43,937 Registered Nurses and transformed the results into a simple, easily interpreted table. 
We transposed the data frame to replicate the table in the original report. For our last steps before merging the data frames, we converted all data types for each attribute to be float. Then saved the cleaned data into clean_webscraped.csv. 


2.2 2022 Survey Data 

The second data source we will use in this project is Employee Attrition for Healthcare dataset from Kaggle, derived from 2022 NSI National Health Care Retention Report. This data shows survey data from 272 hospitals across 32 states. This survey covers 589,901 healthcare workers, and 166,087 Registered Nurses. We created a data frame by importing the raw_2022.csv into 01_kaggle.ipynb that can be found in our project folder. There was not much cleaning needed for this dataset. However, we did drop columns containing factors not recorded in the 2018 data and changed all data types to float. After cleaning and transforming we converted the data frame into clean_kaggle.csv file. 

 2.3 Combining 2018 and 2022 Data

To ensure seamless integration, during the cleaning stages of each source, we confirmed each data frame had the same data types and variables. A description of each variable is listed in Table 1, 2 and 3.  
The format was crucial in order for us to be able to merge the datasets. The data we web scraped was a table that took averages/count from all the survey results. By pulling key factors and calculating the averages/count from our Kaggle dataset, we were able to create identical tables. For this analysis we decided to use the merged data frame to see the overall differences between 2018 and 2022 attrition trends.

Once both data frames were transposed and calculated into similar tables, we renamed all the columns by adding the year the responses were pulled from, for example: overtime_2018 and overtime_2022. Then created a union merger between both datasets, this combined and showed all columns/rows for both datasets. In the merge_df, there is data comparing factors contributing to attrition rates, before and after COVID-19. Lastly, once we merged, we rounded each data point to two decimal places and downloaded the results into merged.csv file. 




---
