# Data Job Market Analysis 
# Introduction 
A focus on data jobs that are ideal for entry-level candidates, particularly recent graduates. Through research, I will explore the accesibility of the data job market for individuals starting their careers, identifying opportunities and challenges faced by newcomers in the data industry. Additionally, I examine the flexibility of working options available, such as the ability to choose working hours.

### Table of contents 

- [Project overview](#Project-overview)
- [Tools Used](#Tools_Used)
- [Data Sources](#Data-Sources)
- [The Analysis + Insights](#The-Analysis+Insights)
- [Conclusion](#Conclusion)
- [References](#References)


### Project Overview 
As a graduate looking to enter the competitive data job market, I found myself researching the different job roles available and the different working types available. I was inspired by Luke Barousse's analysis of the data job market and the key skills in demand. He concluded that Python was the best skill for beginners to learn. This led me to research how accessible the job market actually is for candidates with no/low experience.


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

### The Analysis + Insights 

1) Ideal job for an entry-level/graduate candidate, what salary can they expect? Can they expect to find a remote job with an EN experience level? What locations are the best for EN data candidates?

<img width="869" alt="image" src="https://github.com/user-attachments/assets/d060ba37-2b66-4e0e-90fa-6023b0be6557">

_Using Sqliteviz_

We can see that:
- The highest paying jobs were all in the USA, with entry level jobs starting at $90,000.00. I had assumed they would all be data analyst roles, however there is also a Data Scienctist and Data Science Consultant role. I placed 'L' - large company as another criteria as it is more realistic for larger companies to hire entry level candidates and pay a high salary.
  

To personalise this and look for a data job that would be ideal for me, I executed this criteria:

<img width="1419" alt="image" src="https://github.com/user-attachments/assets/bd7b268e-026a-475c-9269-acd32e0f17a5">  

_Using Sqliteviz, ideal top 5 jobs based on my criteria_

2) How likely is it that a candidate with no formal experience will be able to find a remote job?

It seems as though the remote ratio (RR) is high just by looking at the data set. The likelyhood of finding a remote job is 78.95% as 480 jobs are still available out of the 608 job records, once we filter out companies with a 0 RR. However, this does not take into consideration the experience level. Once we filter out experience levels above entry level, the percentage drops significantly. 
480 then drops to 74, out of 608 job records, 12.17%. 

We can also look at the sum of the remote ratios and see what types of data roles are likely to be remote:

<img width="800" alt="Screenshot 2024-09-26 at 12 50 44" src="https://github.com/user-attachments/assets/6f868d99-fc67-44fc-aa0a-9183760fe776">

_Data Roles and their remote ratios, using the sum of the remote ratios for each role_


It is significantly harder for a entry level/graduate candidate to land a remote job within Data. This is due to remote jobs usually being reserved for Data engineers and Machine Learning engineers, jobs requiring years of experience. 


<img width="564" alt="image" src="https://github.com/user-attachments/assets/f9c9adc7-389e-4d72-8dec-98189d9c6b70">


_A pivot table showing remote jobs are usually reserved for more senior roles_

### Conclusion
In summary, my analysis of the data job market for entry-level candidates reveals both promising opportunities as well as significant challenges. Whilst there are high-paying entry roles, such as Data Scientist and Data Science Consulatant, these positions are often competitive and mostly available in larger companies. 

It then becomes more difficult if the candidate prefers remote work, the data indicates that while 79% of available jobs may be remote, only about 12% of these will consider candidates with no formal experience. 

### References 
Luke Barousse, _SQL Project Data Job Analysis_, 2024 
- https://github.com/lukebarousse/SQL_Project_Data_Job_Analysis/blob/main/README.md
  Inspired by Luke Barousse's analysis of the data job market and the key skills in demand, I was intrigued by his conclusion that Python is the most valuable skill for data roles. However, what fascinated me further was how this analysis might change when focusing specifically on the accessibility of the job market for entry-level/graduate candidates——those who may not yet possess the advanced skills often sought by recruiters. 

Ruchi, Bhatia, _Data Science Job Salaries_, 2022
- https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries

Thank you for reading!
