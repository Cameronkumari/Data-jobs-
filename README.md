# Data Job Market Analysis 
# Introduction 
A focus on data jobs that are ideal for entry-level candidates, particularly recent graduates. Through research, I will explore the accesibility of the data job market for individuals starting their careers, identifying opportunities and challenges faced by newcomers in the data industry. Additionally, I examine the flexibility of working options available, such as the ability to choose working hours and locations.

### Table of contents 

- [Project overview](#Project-overview)
- [Tools Used](#Tools_Used)
- [Data Sources](#Data-Sources)
- [The Analysis + Insights](#The-Analysis+Insights)
- [Conclusion](#Conclusion)
- [References](#References)


### Project Overview 

### Tools Used 
- Sqliteviz
- Excel
- Kaggle
- RAWGraphs/ RawGraphs 2.0 

### Data Sources 

RAW Dataset: https://1drv.ms/x/c/103f3750a8aa74c2/EWtfqQS1PBZIosK9jr32M3cBs8NTHj8cKcs_tD1FbVtJlw

CLEAN Dataset:
https://1drv.ms/x/c/103f3750a8aa74c2/Eab1dnlkpr9Br0NNTfgSfCsBFxG3dlPITKEQmq3u9lfmPw

Cleaning process 
1. Checked for blanks/errors
2. Removed Column A - rows are numbered by default
3. Made employment types more readable e.g. FL - Freelance, CT - contract
4. Added currency symbols for column G
5. Conditional formatting for cells containing 'EN' highlighting how many jobs are suitable for candidates with low/no experience. (EN - Entry level/Junior positions)

### The Analysis 

How likely is it that a candidate with no formal experience will be able to find a remote job?

It seems as though the remote ratio (RR) is high just by looking at the data set. The likelyhood of finding a remote job is 78.95% as 480 jobs are still available out of the 608 job records, once we filter out companies with a 0 RR. However, this does not take into consideration the experience level. Once we filter out experience levels above entry level, the percentage drops significantly. 

480  then drops to 74, out of 608 job records, 12.17%. 

**Insight 1:** It is significantly harder for a entry level/graduate candidate to land a remote job within Data. 

### References 
Luke Barousse, _SQL Project Data Job Analysis_, 2024 
- https://github.com/lukebarousse/SQL_Project_Data_Job_Analysis/blob/main/README.md
  Inspired by Luke Barousse's analysis of the data job market and the key skills in demand, I was intrigued by his conclusion that Python is the most valuable skill for data roles. However, what fascinated me further was how this analysis might change when focusing specifically on the accessibility of the job market for entry-level/graduate candidates——those who may not yet possess the advanced skills often sought by recruiters. 

Ruchi, Bhatia, _Data Science Job Salaries_, 2022
- https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries
