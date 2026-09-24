## 📌 Project Overview

This project is an **HR Attrition Analytics solution built using Microsoft Fabric and Power BI**.

The project uses the **IBM HR Attrition dataset** to explore employee attrition patterns and demonstrate an end-to-end analytics workflow:

**Data ingestion → Data transformation → Lakehouse → Semantic model → Power BI dashboard → Data security**

The dashboard provides HR-focused analysis of employee attrition across departments, job roles, salary bands, and other employee attributes.

> **Learning Project:** This is a guided learning project based on a Microsoft Fabric tutorial. The implementation was recreated for learning, portfolio development, and hands-on practice with Microsoft Fabric concepts.

---

## 🎯 Business Objective

Employee attrition can create recruitment costs, productivity challenges, and workforce planning issues.

This project helps HR stakeholders explore questions such as:

- What is the overall employee attrition rate?
- How many employees have left the organization?
- Which departments have higher attrition?
- Which job roles show higher employee turnover?
- How does attrition vary across salary bands?
- What employee segments can be explored for deeper analysis?
- How can sensitive HR information be protected?

The dashboard is designed to turn employee-level data into an easy-to-understand HR reporting solution.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| **Microsoft Fabric** | End-to-end analytics platform |
| **Dataflows Gen2** | Data ingestion and transformation |
| **Power Query** | Data cleaning and transformation |
| **OneLake / Lakehouse** | Data storage |
| **Semantic Model** | Analytical layer for reporting |
| **Power BI** | Interactive dashboard |
| **DAX** | KPI and analytical calculations |
| **Column-Level Security (CLS)** | Protection of sensitive data |
| **IBM HR Attrition Dataset** | Source dataset |

---

## 🏗️ Solution Architecture

```text
                IBM HR Attrition Dataset
                         │
                         ▼
                  Dataflows Gen2
                         │
                         ▼
                  Power Query / ETL
                         │
                         ▼
                    Fabric Lakehouse
                         │
                         ▼
                    Semantic Model
                         │
                         ▼
                      Power BI
                         │
              ┌──────────┴──────────┐
              ▼                     ▼
        HR Dashboard          Business Analysis
              │
              ▼
      Data Governance
      & Column-Level Security
```

---

## 🔄 Data Pipeline

### 1. Data Ingestion

The HR dataset is ingested using **Dataflows Gen2** in Microsoft Fabric.

Dataflows Gen2 provides a Power Query-based interface for preparing and loading data without requiring extensive code.

### 2. Data Transformation

Power Query is used to prepare the employee data for analysis.

The transformation workflow includes:

- Data type validation
- Column preparation
- Data cleaning
- Creating analytical categories
- Creating salary bands
- Creating age groups
- Preparing fields for reporting

### 3. Lakehouse

The transformed data is loaded into a **Microsoft Fabric Lakehouse**.

The Lakehouse provides a centralized storage layer that can be used by downstream analytical workloads.

### 4. Semantic Model

The prepared data is exposed through a **semantic model** for reporting and analytical queries.

The semantic layer supports:

- Measures
- KPI calculations
- Filtering
- Aggregations
- Interactive Power BI analysis

### 5. Power BI Dashboard

Power BI is used to build an interactive HR Attrition dashboard containing KPI cards, charts, tables, and a decomposition tree.

---

# 📊 Dashboard

The report contains an overview page focused on workforce attrition.

### Key metrics shown

- **Attrition Rate**
- **Employees Left**
- **Total Headcount**
- **Average Income**
- **Average Tenure of Leavers**

### Main visualizations

- Attrition by Department
- Attrition Decomposition
- Attrition by Job Role
- Attrition by Salary Band
- Overall Attrition
- Interactive slicers for Department, Gender, and Salary Band

### Dashboard Screenshot

![HR Attrition Dashboard](Screenshots/dashboard.png)

---

# 🔐 Data Governance & Security

HR analytics can involve sensitive employee information. Therefore, the project also demonstrates a data governance and security concept using **Column-Level Security (CLS)**.

Sensitive information such as **Monthly Income** can be restricted so that users without the required permissions cannot access protected columns.

### Security implementation

The project demonstrates:

- Lakehouse security roles
- Data access permissions
- Column-Level Security constraints
- Protection of sensitive employee information

### Security Screenshot

![Column-Level Security](Screenshots/column-level-security.png)

---

# 🗄️ Lakehouse

The transformed `hr_employees` table is stored in the Fabric Lakehouse and can be used as the source for the analytical layer.

### Lakehouse Screenshot

![Microsoft Fabric Lakehouse](Screenshots/lakehouse.png)

---

# 📈 Analytical Areas

The dashboard allows users to explore attrition across several dimensions, including:

- Department
- Job Role
- Salary Band
- Gender
- Age
- Job Level
- Job Satisfaction
- Overtime
- Business Travel
- Years at Company
- Monthly Income

These dimensions are used to identify **patterns and segments associated with employee attrition**. They should not be interpreted as proof that a particular factor directly causes employees to leave.

---

# 💡 Business Insights

The dashboard can be used to identify patterns such as:

- Differences in attrition rates between departments
- Job roles with comparatively higher attrition
- Attrition variation across salary bands
- Employee groups requiring deeper investigation
- Overall workforce retention patterns

For example, the sample dashboard shows an overall attrition rate of **16.1%**, with **237 employees left out of a total headcount of 1,470** in the displayed dataset.

These figures are descriptive results from the project dataset and are not intended to represent a real organization's current HR statistics.

---

# 📚 Microsoft Fabric Concepts Demonstrated

This project provides hands-on practice with:

- Microsoft Fabric
- Dataflows Gen2
- Power Query
- OneLake
- Lakehouse
- Semantic Models
- Power BI
- DAX
- Data transformation
- Data governance
- Column-Level Security
- End-to-end analytics workflow

---

# 📁 Repository Structure

```text
HR-Attrition-Microsoft-Fabric/
│
├── README.md
│
└── Screenshots/
    ├── 01-lakehouse.png
    ├── 02-column-level-security.png
    └── 03-dashboard.png
```

If Fabric project artifacts or exported files are added later, they can be organized into additional folders such as:

```text
├── Fabric/
├── Dataset/
├── PowerBI/
└── Documentation/
```

---

# 🎓 Key Learning Outcomes

Through this project, I practiced:

- Building a data ingestion pipeline with Dataflows Gen2
- Transforming data using Power Query
- Working with a Fabric Lakehouse
- Understanding the role of a semantic model
- Creating Power BI dashboards
- Writing analytical DAX measures
- Designing business-focused KPI reporting
- Using decomposition trees for exploratory analysis
- Applying data governance concepts
- Implementing Column-Level Security
- Connecting technical implementation with a business use case

---

# 🎥 Tutorial Reference

This repository is based on a guided Microsoft Fabric HR Attrition project tutorial.

The project has been recreated for **learning and portfolio purposes**, with the implementation documented through screenshots and project notes.

---

# 👨‍💻 Author

**Nishant Kumar**

Aspiring Data Analyst | Power BI | SQL | Python | Microsoft Fabric

---

## ⭐ Project Focus

**Microsoft Fabric · Dataflows Gen2 · Power Query · Lakehouse · Semantic Model · Power BI · DAX · Data Governance · Column-Level Security**
