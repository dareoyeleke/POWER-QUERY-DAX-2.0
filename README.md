# POWER-QUERY-DAX-2.0
Creating Visuals was just the beginning. Power Query and DAX have taken things a step further giving me more control over manipulating my data. The steps along with screenshots of visual will help you through mu journey through DAX and power query and the skills used as well as insights found with this project. My full prject on core visuals along with the dashboard can be viewed at this link https://github.com/dareoyeleke/power_bi_dashboard_and_visuals-


# 📊 Data Jobs Analytics Dashboard (Power BI + Power Query + DAX)
### 🧾 Overview

This project analyzes the data science and analytics job market using Power BI, with emphasis on:

🧱→🔧→📊 Power Query (ETL and Data shaping) 

📐 DAX for analytics and KPI modeling (Aggregations, measures, parameters,columns, tables) 

🗃️ Dimensional modeling (star schema and relationships)  for performance and clarity

📈 Visual insights into job demand, salaries, and skills

**The dashboard is designed for recruiters, hiring managers, and job seekers to quickly understand what roles pay well, where demand is highest, and which skills matter most.**

### 🎯 Key Business Questions

This dashboard answers questions such as:

-  🔢 How many data roles are currently available?

-  💵 What is the median yearly and hourly salary by role?

-  🧠 Which skills are most in-demand?

-  👨‍💼 Which job titles have the highest value in the market?

-  🌍 How do metrics change by country and job position?

### 📊 Dashboard Highlights
-  🧍‍♂️ KPIs

-  479K job postings

-  $113K median annual salary

-  $99/hour adjusted median hourly rate

-  4.8 skills per job posting

### 📌 Skills Analysis

Shows the top skills in data, ranked by frequency:

-  Python

-  SQL

-  AWS

-  Azure

-  Tableau

-  Spark
...and more

### 💡 Provides insight into which skills drive the most job opportunities.

### 💰 Salary Analysis

**Breaks down median yearly salary by role:** 

-  Senior Data Scientist

-  ML Engineer

-  Data Engineer

-  Software Engineer

-  Cloud Engineer

-  Data Analyst
...etc.

**💡 Helps identify the most lucrative roles in the market.**

**🔍 Interactive Filters**

### Users can filter by:

-  🌎 Country

-  🧑‍💼 Job position

…and recalibrate KPIs and charts instantly.

### 🧩 Data Model

**This solution uses a star schema optimized for analytics.**

### 🌟 Fact Table

**job_postings_fact (central table)**

**📚 Dimensions**

-  job_title_dim

-  skills_dim

-  skills_job_dim

-  company_dim

-  schedule_dim

-  date_dim

-  countries

### 🔢 Parameter & Helper Tables

**Used for:**

-  Dynamic filtering

-  Controlled slicers

-  Numeric evaluation

-  Parameterized ranking

**🔑 Relationships are one-to-many, many-to-one and one-to-one enforcing referential integrity and reducing ambiguity.**

### 🔧 Power Query (ETL) Work

**Automated transformations include:**

-  Data type standardization

-  Creation and manipulation of  fact, dim and then flat tables from star schema 

-  Column extraction and splitting with delimeters, pivoting with key/value attributes, and sorting/filtering rows

-  Merging tables on business keys

-  Null/error handling

-  Standardized salary calculation logic

**💡 Focus: Create a clean, reusable, refreshable pipeline.**

### 🧮 DAX Measures (Analytics Layer)

**This project leverages measure branching and DAX patterns for:**

-  📅 Time intelligence

-  📊 KPI calculations

-  🧮 Aggregation logic

-  📌 Percent of total metrics

**Key measures include:**

-  Job Count

-  Median Yearly Salary

-  Median Hourly Salary ADJ

-  Skill Count

-  Skill Per Job

-  Job Percentage

**💡 Measures are optimized to scale with new data and additional dimensions.**

### 🚀 Performance Design Choices

-  Star schema

-  Optimized cardinality

-  Measure-based logic (not calculated columns)

-  Disabled auto date hierarchy

-  Custom parameter tables for controlled interactions

-  Use DAX functions to operate at row, query and filter contexts
  - Functions like CALCULATE, SUM, SUMX, FILTER, ALL, ALLEXCEPT, FORMAT(date/time), CALENDAR, CALENDAR AUTO. e.t.c were utilized to this effect       

💡 Designed for speed, maintainability, and clarity.

### 🖥️ How to Use

-  Open the .pbix file in Power BI Desktop

-  Connect / update source data if needed

-  Refresh to populate updated metrics

-  Filter by country or job role to explore insights

### 📌 Value Proposition

**This project demonstrates ability to:**

-  Streamline messy data into analytical tables

-  Engineer DAX solutions ( expressions, parameter, measures. e.t.c) to answer business questions

-  Build intuitive, interactive dashboards

-  Model data with scalable, enterprise-ready architecture
  

**💡 Not just visuals — a full analytics product.**

🔭 Future Enhancements

Possible upgrades:

Role-level security for controlled access

Incremental data refresh

Advanced time-series forecasting

Skill clustering / recommendation engine

# 📬 Contact

### For collaboration or opportunities:
-  Email: oyesope@gmail.com
-  LinkedIn: https://www.linkedin.com/public-profile/settings?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_self_edit_contact-info%3BrEJT%2B0LuT3uhIlpIujK1IQ%3D%3D


# CONCLUSION 💡
```
  The visuals below show how applying Power BI through power query and DAX can transform messy data and give insighful answers
to questions about the job market. Navigating potential career paths can be difficult, but with structured and arranged insights
like this, it's definitely less difficult to create informed decisions when facing a bulk of data such as these job postings  
```

# 📎 Screenshots of Visuals
### 🖼️ Dashboard

```
  This visual is a summary representation of the job market, showcasing key performance indicators like Job Count, Skills per job,
Median Yearly Salary, Median Hourly Salary adjudted to the year, side by side metrics for both and the percentages for jobs.
Overall the Dashboard is designed for efficient navigation, with included slicers and bookarks to drill down to specific jobs,
countries and a combination of multiple at the same time, and/or effectively clear the selections to start fresh if needed.  
```

<img width="1920" height="1080" alt="QUERY DAX DASH 2 0" src="https://github.com/user-attachments/assets/4c2f646f-311c-408f-863a-f41a79d20bab" />




### 🗺️ Data Model
```
  The data model here, shows the flat table, i.e the main table (job_postings_fact) and every dimensional table created from it
as well.All parameters, both numerical and field are shown, as well as measures used throughout the project.
While the numerical parameter isn't used in the Dashboard, the visual below shows its application.   
```
  <img width="1920" height="1016" alt="tables, measures, parameters model" src="https://github.com/user-attachments/assets/2dfe3eb7-3cb4-4263-bb37-5f45f5b16c20" />


### Worthy of Mention ⭐
**Visual with Numeric parameter to visualize tax deductions at different rates for Yearly and Hourly Salary adjusted to the year for multiple positions** 

```
  The numerical parameter indicated above was used in combination to create this visual with frequently used metrics.
Those metris were made into aggregate measures for quick access to compare US specific hourly salaries adjusted to a full year.
A full year being 52 40 hour weeks and yearly salaries, with a side by side numerical parameter to compare different deduction
rates with a sliding scale or tax rate input
```

<img width="1920" height="1080" alt="QUERY DAX 11" src="https://github.com/user-attachments/assets/b16b5471-0448-4942-af09-6fa783b5ba40" />

