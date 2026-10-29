## MySQL Healthcare Project

The dataset represents 10 years (1999-2008) of Clinical care at 130 US hospitals. Each row is a patient diagnosed with diabetes, and performed laboratory testing, medications, and stayed up to 14 days in the hospital. The dataset is made up of two tables, the health table consisting of 101,766 rows of patient encounters/admission to the hospital, and the demographics table consisting of 71,518 rows of patient details. [Click here to access the dataset](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008). 

What is the distribution of time spent in the hospital, and do the majority of patients stay less than 7 days? Using the following query, it looks like 80,617 (79%) of patients stay less than 7 days in the hospital, while the remaining 21,149 (21%) stayed more than 7 days.  

### 1. Use this SQL query: 
```python
'USE patient, 
SELECT ROUND (time_in_hospital,1) AS number_of_days_spent_in_hospital, 
COUNT (*) AS admission_count, 
RPAD (' ', COUNT (*)/1000, '*') AS bar 
FROM health 
GROUP BY  number_of_days_spent_in_hospital 
ORDER BY number_of_days_spent_in_hospital; 
```



