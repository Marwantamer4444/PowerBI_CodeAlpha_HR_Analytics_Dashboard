# CodeAlpha_HR_Analytics_Dashboard

## Project Title

**Human Resources Analytics Dashboard using Power BI**

## Internship Domain

**Power BI Internship — CodeAlpha**

## Task

**Task 2: Human Resources Analytics**

## Project Overview

This project is an interactive **Human Resources Analytics Dashboard** developed using **Microsoft Power BI**.
The dashboard analyzes employee data to help HR teams understand workforce distribution, employee attrition, satisfaction levels, performance ratings, and hiring needs.

The goal of this project is to support HR decision-making by transforming raw employee data into clear visual insights.

---

## Objective

The main objective of this dashboard is to analyze and optimize HR processes and workforce management by:

* Tracking employee turnover and attrition rates
* Analyzing workforce distribution by department and gender
* Studying employee satisfaction and performance
* Identifying job roles with high attrition
* Supporting hiring and retention planning through department-level insights

---

## Dataset Used

The dataset used in this project is the **IBM HR Employee Attrition Dataset**.

The dataset contains employee-related information such as:

* Age
* Gender
* Department
* Job Role
* Monthly Income
* Attrition
* Job Satisfaction
* Performance Rating
* Years at Company
* Work-Life Balance
* Business Travel
* Distance from Home
* Marital Status
* Environment Satisfaction
* Training Times Last Year

---

## Tools and Technologies

The following tools were used to complete this project:

* **Power BI Desktop**
* **Power Query**
* **DAX**
* **Excel / CSV Dataset**
* **Data Visualization**
* **HR Analytics**

---

## Dashboard Pages

The Power BI report contains two main pages:

---

# Page 1: Workforce Overview

This page provides a general overview of employee distribution and attrition.

## Key Performance Indicators

The dashboard includes the following KPI cards:

| KPI                    | Description                                  |
| ---------------------- | -------------------------------------------- |
| Total Employees        | Total number of employees in the dataset     |
| Attrition Rate         | Percentage of employees who left the company |
| Average Age            | Average age of employees                     |
| Average Monthly Income | Average monthly income of employees          |

## Visualizations

This page includes:

### 1. Employees by Department

Shows the total number of employees in each department.

### 2. Attrition by Department

Shows the number of employees who left the company in each department.

### 3. Attrition Rate by Department

Shows the attrition percentage for each department.

### 4. Employees by Gender

Shows the gender distribution of employees.

### 5. Attrition by Gender

Shows employee attrition distribution by gender.

### 6. Interactive Filters

The report includes slicers for:

* Department
* Gender

These filters allow users to interact with the dashboard and analyze specific employee groups.

---

# Page 2: Satisfaction & Hiring Forecast

This page focuses on satisfaction, performance, job role attrition, and hiring risk.

## Visualizations

### 1. Average Job Satisfaction by Department

Shows the average job satisfaction score across departments.

### 2. Average Performance Rating by Department

Shows the average performance rating for each department.

### 3. Attrition by Job Role

Shows which job roles have the highest number of employees leaving the company.

### 4. Hiring Need Forecast by Department

A summary table showing:

* Department
* Total Employees
* Attrition Count
* Attrition Rate
* Average Monthly Income

This table helps identify departments that may require stronger hiring or retention planning.

---

## DAX Measures Used

The following DAX measures were created in Power BI:

### Total Employees

```DAX
Total Employees = COUNTROWS('WA_Fn-UseC_-HR-Employee-Attrition (2)')
```

### Attrition Count

```DAX
Attrition Count =
CALCULATE(
    COUNTROWS('WA_Fn-UseC_-HR-Employee-Attrition (2)'),
    'WA_Fn-UseC_-HR-Employee-Attrition (2)'[Attrition] = "Yes"
)
```

### Attrition Rate

```DAX
Attrition Rate =
DIVIDE(
    [Attrition Count],
    [Total Employees]
)
```

### Average Monthly Income

```DAX
Average Monthly Income =
AVERAGE('WA_Fn-UseC_-HR-Employee-Attrition (2)'[Monthly Salary])
```

### Average Age

```DAX
Average Age =
AVERAGE('WA_Fn-UseC_-HR-Employee-Attrition (2)'[Age])
```

---

## Key Insights

The dashboard provides the following insights:

* The total number of employees analyzed is **1,470**.
* The overall attrition rate is approximately **16%**.
* **Research & Development** has the highest employee count.
* **Research & Development** also has the highest attrition count because it has the largest workforce size.
* **Sales** has the highest attrition rate, which indicates a higher retention risk.
* Male employees represent around **60%** of the workforce.
* Laboratory Technicians and Sales Executives show high attrition counts by job role.
* Job satisfaction and performance ratings are close across departments, but small differences can still help HR teams identify improvement areas.
* Departments with higher attrition rates may require stronger hiring plans and retention strategies.

---

## Business Value

This dashboard helps HR managers and business leaders to:

* Monitor workforce size and structure
* Identify departments with high attrition
* Understand employee satisfaction and performance trends
* Detect job roles with higher employee turnover
* Make better hiring and retention decisions
* Improve workforce planning using data-driven insights

---

## Project Files

The repository contains:

```text
CodeAlpha_HR_Analytics_Dashboard.pbix
README.md
Dataset file
Dashboard screenshots
```

Recommended folder structure:

```text
CodeAlpha_HR_Analytics_Dashboard/
│
├── CodeAlpha_HR_Analytics_Dashboard.pbix
├── README.md
├── dataset/
│   └── HR_Employee_Attrition.csv
│
└── screenshots/
    ├── workforce_overview.png
    └── satisfaction_hiring_forecast.png
```

---

## Screenshots

### Page 1: Workforce Overview

<img width="1923" height="1090" alt="image" src="https://github.com/user-attachments/assets/bc202dd4-c6fd-4c73-8937-52310933ae83" />


```markdown
![Workforce Overview](screenshots/workforce_overview.png)
```

### Page 2: Satisfaction & Hiring Forecast

<img width="1917" height="1074" alt="image" src="https://github.com/user-attachments/assets/8757cb43-094a-44d2-aee4-15b8ea83a0bc" />


```markdown
![Satisfaction & Hiring Forecast](screenshots/satisfaction_hiring_forecast.png)
```

---

## How to Open the Project

To open and explore the dashboard:

1. Download the `.pbix` file from this repository.
2. Open it using **Microsoft Power BI Desktop**.
3. Use the slicers to filter by department and gender.
4. Navigate between the two report pages:

   * Workforce Overview
   * Satisfaction & Hiring Forecast

---

## Final Deliverable

The final deliverable is an interactive Power BI report that supports HR decision-making through:

* Employee attrition analysis
* Workforce distribution analysis
* Satisfaction and performance tracking
* Hiring need forecasting
* Interactive filtering and visualization

---

## Internship Submission

This project was completed as part of the **CodeAlpha Power BI Internship**.

Repository name format:

```text
CodeAlpha_HR_Analytics_Dashboard
```

---

## Author

**Marwan Tamer**

---

## Tags

`Power BI` `HR Analytics` `Data Analytics` `DAX` `Power Query` `Dashboard` `Business Intelligence` `CodeAlpha`
