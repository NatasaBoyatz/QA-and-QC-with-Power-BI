# QA-and-QC-with-Power-BI

# Quality Assurance and Quality Control with Power BI

### Dashboard Link: https://github.com/NatasaBoyatz/QA-and-QC-with-Power-BI/blob/main/Power%20Bi%20Final.pbix
## About the project

   This project is about the quality control and the employee peformance using data from a small industry.This type of data is commonly used from business and industries to assess and improve performance standards,identify critical errors, and determine areas where training or adjustments are needed.


### Dashboard content explaining


- Step 1 : Load data into Power BI Desktop, dataset is a csv file.

- Step 2 : Create measures Sampling%, Defects%, Fatal Errors% to calculate the percentage of samples over total tasks, defects and fatal errors over samples. Also calculating Quality Score as defects% parameter.

                Dax expressions:

                Sampling% = DIVIDE(SUM('Quality Data'[Samples]), SUM('Quality Data'[Total Task]),0)

                Defects% = DIVIDE(SUM('Quality Data'[Defects]), SUM('Quality Data'[Samples]),0)

                Fatal errors% = DIVIDE(SUM('Quality Data'[Fatal Errors]),SUM('Quality Data'[Samples]),0)
                
                Quality score = 1- [Defects%]


- Step 3 : Display Total Tasks, Samples, Defects, and Fatal Errors using Card graphs.

- Step 4 : Visualize Quality Score to show:


	-Quality Score % (Gauge Chart).

	-Quality Score by Supervisor, with labels showing both category and value (Donat Chart).

	-Quality Score by Work Location (Map Chart).


- Step 5 : Analyze Sampling by Supervisor (%) and Fatal Errors by month, using a Clustered Bar chart and an Area chart respectively.

- Step 6 : Visualize Employee-Level Insights (Samples vs. Defects by EMP Name).

- Step 7 : Creating a new tooltip page named "EMP Tooltip", adding a Clustered Bar chart to show Quality Score (%) by EMP Name and link it to the Samples vs. Defects by EMP Name scatter plot on the Quality Dashboard.

- Step 8 : Finalize Report by adding a Clustered bar chart for Employee Performance by Supervisor, using EMP Name, Supervisor, Quality Score and Defects as fields. 


 
# Snapshot of Quality Dashboard

![Image](https://github.com/user-attachments/assets/d5f7bde9-5996-4b04-b65a-02ac4393877f)

 
 # Snapshot of Employee Performance

 ![Image](https://github.com/user-attachments/assets/ef5d2681-89d7-4f84-a3bb-68d84bfc7ece)
