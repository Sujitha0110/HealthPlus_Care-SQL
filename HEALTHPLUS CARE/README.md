# HealthPlus Care Healthcare Analytics

## Overview
HealthPlus Care is a **SQL/MySQL healthcare analytics project** focused on healthcare service utilization, specialist and clinic performance, member engagement, telemedicine adoption, member satisfaction, and billing and payment collection. The project creates a relational database, inserts healthcare records, performs data profiling and cleaning, and uses SQL queries to generate business-focused insights.

## Objectives
- Analyze member demographics and membership types
- Understand consultation activity and completion rates
- Evaluate clinic workload and specialist performance
- Measure telemedicine adoption and session status
- Analyze laboratory testing activity and costs
- Review member feedback and satisfaction
- Compare billed amounts with successful payments
- Identify data-quality issues and clean inconsistent member information

## Technology Stack
- **Database:** MySQL
- **Language:** SQL
- **Data Source:** Records inserted through SQL `INSERT` statements

## Database
**Database:** `healthpluscare_db`

The project contains **17 tables** covering clinics, specialists, members, corporate accounts and memberships, consultations, telemedicine sessions, chronic care programs, health packages, package subscriptions, prescriptions, lab tests, claims, staff, billing, payments, and feedback.

## Dataset
| Area | Records |
|---|---:|
| Clinics | 18 |
| Specialists | 220 |
| Members | 2,500 |
| Corporates | 60 |
| Corporate Members | 615 |
| Consultations | 6,000 |
| Telemedicine Sessions | 2,200 |
| Chronic Care Programs | 900 |
| Health Packages | 40 |
| Package Subscriptions | 3,000 |
| Prescriptions | 5,000 |
| Lab Tests | 3,500 |
| Claims | 1,800 |
| Staff | 450 |
| Billing | 6,000 |
| Payments | 6,000 |
| Feedback | 2,500 |

*Record counts are based on the `INSERT` statements in the supplied SQL script.*

## Key KPIs and Measures
- Total Members
- Total Consultations
- Completed Consultations
- Consultation Completion Percentage
- Consultation Count by Mode
- Telemedicine Adoption Percentage
- Telemedicine Session Count by Status
- Top Clinics by Consultation Activity
- Specialist Consultation Fee: Average, Minimum, and Maximum
- Total Billed Amount
- Successful Payment Amount
- Collection Percentage
- Collection Gap
- Average Member Feedback Rating
- Total Feedback Records

## Project Workflow
```text
SQL Data and INSERT Statements
          ↓
MySQL Database Creation
          ↓
17 Relational Tables
          ↓
Data Profiling
          ↓
Data Cleaning
          ↓
SQL Practice and Business Analysis
          ↓
KPI Queries
          ↓
Business Insights and Recommendations
```

## Data Profiling and Cleaning
The SQL script checks for the following data-quality issues:

- Inconsistent gender values in the `Members` table
- Missing email values in the `Members` table
- Emails that do not follow the expected email pattern
- Missing consultation IDs in the `Claims` table
- Missing insurance provider values in the `Claims` table
- Missing consultation IDs in the `Billing` table
- Missing payment modes in the `Payments` table

Cleaning operations included:
- Standardizing member gender values to `Male` and `Female`
- Correcting certain email values that were missing the `@` symbol

## SQL Analysis
The project includes SQL practice queries and presentation-focused analysis using:
- Aggregate functions: `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`
- Grouping and filtering: `GROUP BY`, `HAVING`, `ORDER BY`, `LIMIT`
- Joins: `INNER JOIN`, `LEFT JOIN`
- Subqueries
- Conditional logic: `CASE`
- String functions: `CONCAT()`, `LOWER()`, `TRIM()`, `REPLACE()`
- Window functions: `RANK()`, `LEAD()`, `LAG()`

## Business Analysis
The presentation queries investigate:
- Overall healthcare activity and completed consultations
- Clinics with the highest consultation volumes
- Members with the highest consultation activity
- Telemedicine usage and session status
- Average member feedback rating
- Consultation completion percentage
- Total billed value and successful recorded payments
- Collection percentage and collection gap
- Bill status distribution

## Project Files
```text
HealthPlus-Care/
└── healthpluscare_database.sql
```

The SQL file includes database creation, table creation, data insertion, data profiling, data cleaning, SQL practice questions, and presentation/business analysis queries.

## Outcome
The project transforms healthcare records into **structured SQL analysis, operational KPIs, and business insights**. It supports understanding of clinic and specialist activity, member engagement, virtual-care usage, member satisfaction, and billing-to-payment performance.

**Project Type:** Academic / Data Analytics Project  
**Domain:** Healthcare Analytics  
**Database:** MySQL
