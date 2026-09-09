# IBM HR Analytics – Employee Attrition Dashboard

## 1. Project Title 
IBM HR Analytics Attrition Dashboard

## 2. Short Description
A Power BI dashboard analyzing **employee attrition** using the IBM HR Analytics dataset. It covers attrition rate, department/job-role trends, and key drivers like overtime, travel, distance from home, salary hike, and job satisfaction — with demographic filters for deeper analysis.

## 3. Tech Stack
- MySQL (data staging & querying)
- Power BI Desktop
- Power Query
- DAX
- Data Modeling
- .pbix / .png

## 4. Data Source & Pipeline
**Source:** IBM HR Analytics Employee Attrition dataset (Kaggle, CSV)

**Workflow:**
1. Dataset downloaded from Kaggle as a `.csv` file
2. Loaded into a MySQL database (`Employees` table) using `LOAD DATA LOCAL INFILE`
3. Queried and validated in MySQL
4. Connected to Power BI for modeling and visualization

Employee-level fields include:
- Demographics (Gender, Age, Marital Status)
- Job Role, Job Level, Department, Salary
- Job/Environment Satisfaction, Involvement, Work-Life Balance
- Overtime, Business Travel, Distance from Office
- Education, Salary Hike %, Total Working Years, Years at Company/Current Role
- Attrition status

## 5. Highlights

### i. Business Problem
With 10,000 employees across departments and job roles, IBM needed a clear way to identify **where and why attrition is happening**, and which employee segments are most at risk.

### ii. Goal of the Dashboard
- Track overall attrition rate and headcount
- Compare attrition across departments and job roles
- Identify key drivers: overtime, travel, distance, salary hike
- Analyze satisfaction, involvement, and work-life balance scores
- Enable filtering by gender, job role, and job level

### iii. Key Visuals

**KPI Overview**
- 10,000 Total Employees
- 2,247 Total Attrition
- 7,753 Active Employees
- 22.47% Attrition Rate
- 40 Average Age

**Attrition vs Total Employees**
- Trend comparison across departments: Cyber Security, Software Development, Data Science, IT Services, Network Administration

**Attrition Drivers**
- By Overtime: No (1,449, ~64%) vs Yes (798, ~36%)
- By Business Travel: Rarely (1,182), Frequently (690), No Travel (375)
- By Distance from Home: rising attrition with distance
- By Salary Hike %: fairly evenly spread across hike bands
- By Years in Current Role: fluctuating, peak around year 4–5

**Attrition by Department**
- Cyber Security (503, 22.4%), Software Development (462, ~20.6%), Data Science (442, 19.7%), Network Administration (410, 18.2%), IT Services (430, ~19.1%)

**Attrition by Education**
- Graduate (702), Degree (686), Master's (438), PhD (221), Below College (200)

**Attrition by Job Role**
- Highest: Consultant (208), Director (199), QA Analyst (199), IT (198)
- Others: Business roles, Software Dev, Help Desk, Technician, HR, Manager, Developer, Support (174–186 range)

**Filters**
- Gender, Job Role, Job Level

### iv. Business Impact
- Pinpoints high-attrition departments and job roles
- Flags overtime and travel as major attrition drivers
- Highlights how distance from home correlates with attrition
- Surfaces low satisfaction/involvement/work-life balance segments
- Supports targeted retention strategies for HR

## 6. Screenshots

### i. Overview Dashboard
KPI summary and department-level attrition vs total employee trend.

<img width="603" height="370" alt="IBM HR Analytics Dashboard - Overview" src="Employee_Attrition_Overview.png" />

### ii. Attrition Drivers & Demographics
Breakdown of attrition by overtime, travel, distance, salary hike, department, education, and job role, with gender/job role/job level filters.

<img width="603" height="370" alt="IBM HR Analytics Dashboard - Drivers & Demographics" src="Attrition_Drivers___Demographics.png" />
