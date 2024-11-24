# **Netflix Userbase Analytics**

## **Introduction**
The *Netflix Userbase Analytics* project delivers a comprehensive analysis of Netflix's user behavior and content trends using publicly available datasets. By leveraging modern data engineering and analytics tools, the project aims to uncover actionable insights into customer preferences, subscription patterns, and content popularity. These insights can help OTT platforms like Netflix make data-driven decisions to optimize their services and grow their userbase.

---

## **Project Overview**
### **Objectives**
This project addresses key questions for Netflix’s business strategy, including:
1. Understanding subscription patterns:
   - Subscription plans by user demographics.
   - Monthly revenue generation trends.
2. Analyzing content consumption:
   - Device usage for streaming.
   - Most-watched genres, directors, and actors.
3. Assessing Netflix’s growth areas:
   - Preferences between movies and TV shows.
   - Regional content performance.

### **Workflow**
1. **Data Sources:**
   - [Netflix Userbase Dataset](https://www.kaggle.com/datasets/arnavsmayan/netflix-userbase-dataset/code)
   - [Netflix Shows Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)
   - [IMDB Datasets](https://datasets.imdbws.com/)

2. **Data Collection & Storage:**
   - Raw data is stored in AWS S3 buckets for centralized management.

3. **Data Transformation & Extraction:**
   - AWS Glue and PySpark are used to clean, transform, and enrich data.

4. **Data Loading:**
   - Transformed data is loaded into an AWS RDS (PostgreSQL) data warehouse.

5. **Visualization:**
   - Interactive dashboards created in Tableau visualize key insights and KPIs.

![image](https://github.com/user-attachments/assets/624c49f3-e856-4732-92c7-747ae6d19393)


---

## **Data Architecture**
### **Steps**
1. **S3 Buckets:** 
   - CSV files are organized into folders within S3 buckets.  

2. **AWS Glue ETL Jobs:**
   - Crawlers scan datasets to populate the AWS Glue Data Catalog.
   - PySpark scripts handle dimension and fact table transformations.  

![image](https://github.com/user-attachments/assets/c69a0525-4e61-413b-84af-605eb5473241)

![image](https://github.com/user-attachments/assets/f989ad06-b66f-45c6-812b-49f576339b33)



3. **Data Warehouse:**
   - Processed data is stored in a RDS star-schema format for OLAP analysis.  

![image](https://github.com/user-attachments/assets/acb7f09c-0525-42ec-b1b7-5e79c46b631d)

![image](https://github.com/user-attachments/assets/993acdbc-8f19-4b94-9061-31c83890ea9d)



4. **Automation:**
   - AWS Glue workflows automate the ETL process end-to-end.  

![image](https://github.com/user-attachments/assets/dfce0127-242e-483a-bd52-bfab3e166fcc)


5. **Dashboards:**
   - Tableau dashboards showcase key insights like user preferences and revenue trends.  

![image](https://github.com/user-attachments/assets/92888332-3b7b-46fe-b56b-b85c1e230168)



---

## **Conclusion**
This project equips stakeholders with actionable insights into Netflix's userbase and content strategy. By leveraging modern data analytics and cloud technologies, it demonstrates how data-driven decision-making can enhance customer satisfaction and business growth.
