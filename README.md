Hospital Emergency Room Dashboard
Dashboard Link: https://drive.google.com/file/d/1uTf9O4RqmWNrIzBO5UIR0d5aXEGAufV_/view?usp=sharing

[Dashboard Overview]:

![overview_page-0001](https://github.com/user-attachments/assets/207e8769-a53d-4def-89d6-d2047a1f3483)




Problem Statement
The Hospital Emergency Room Dashboard provides an in-depth analysis of emergency room operations over a 19-month period (April 2023 – October 2024), covering 9,216 unique patient records.
It helps hospital management monitor patient volumes, wait times, satisfaction scores, referrals, demographics, and admission patterns.

Insights from this dashboard guide resource allocation, optimize staff scheduling, improve patient throughput, and enhance the patient experience.



Steps Followed
1.  Requirement Gathering  with hospital administrators to identify KPIs.  
2.  Data Walkthrough  to validate sources and understand field definitions.  
3.  Data Connection  to hospital EMR & operational databases.  
4.  Data Cleaning  & quality checks to remove nulls and inconsistencies.  
5.  Data Modeling  to link patient, department, and time dimensions.  
6.  Data Processing  for analysis-ready tables.  
7.  DAX Calculations  for KPIs like patient counts, average wait times, and satisfaction.  
8.  Dashboard Layouting  to ensure clarity and usability.  
9.  Chart Development  for trends, breakdowns, and comparisons.  
10. Publishing  to Power BI Service for accessibility.


Dashboards Created

1.Monthly View
2.Consolidated View
3.Patient Details
4.Key Takeaways


1. Monthly View
Objective: Track ER activity month-by-month to identify patterns and gaps.

Monthly View: 

![overview_page-0001](https://github.com/user-attachments/assets/f50b676a-3a4a-4829-be37-7db9b6aae45a)



Example (Feb 2024):

Patients: 431
Avg Wait Time: 36.7 mins
Avg Satisfaction: 4.72 / 10
Patients Referred: 179
Admitted: 224 (51.97%)
Seen within 30 mins: 65.66%




2. Consolidated View
Objective: Provide aggregated KPIs over any date range.

Consolidated View:

<img width="1736" height="1070" alt="image" src="https://github.com/user-attachments/assets/9fa9ba9b-81da-4ecf-815f-0e55749a95dc" />


Example (Apr 2023 – Aug 2024):

Patients: 7,982
Avg Wait Time: 35.3 mins
Avg Satisfaction: 4.96 / 10
Admitted: 3,987 (49.95%)
Not Admitted: 3,995 (50.05%)
Seen within 30 mins: 59.4%




3. Patient Details
Objective: Provide granular records for detailed analysis.

Patient Details

<img width="1727" height="1070" alt="image" src="https://github.com/user-attachments/assets/acd1037d-7008-4ca2-b26c-347b677f407e" />


Fields: Patient ID, Name, Gender, Age, Admission Date, Wait Time, Referral Dept, Admission Status.




4. Key Takeaways
Objective: Summarize findings into actionable points.

Key Takeaways

<img width="1736" height="1066" alt="image" src="https://github.com/user-attachments/assets/8b8bade6-6d23-475d-8878-e59bef61f19f" />


Highlights:

Total Patients: 9,216
Avg Wait Time: 35.3 mins
Avg Satisfaction: 4.99 / 10
Top Referrals:
General Practice – 1,840
Orthopedics – 995
Physiotherapy – 276
Cardiology – 248
Busiest Days: Monday (1,377), Saturday (1,322), Tuesday (1,318)
Busiest Hours: 11 AM, 1 PM, 7 PM, 11 PM
Largest Age Group: 30–39 years (1,200 patients)
Largest Race Group: White (2,571 patients)
Admission Split: 4,612 admitted vs 4,604 not admitted




Example DAX Measures

Total Patients = COUNT(Patients[Patient ID])

Average Wait Time = AVERAGE(Patients[Wait Time])

Average Satisfaction = AVERAGE(Patients[Satisfaction Score])

Referral Count = COUNT(Patients[Department Referral])


Portfolio: https://amithgowda.netlify.app/

