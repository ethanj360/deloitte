# Deloitte Australia Data Analytics Case Study
### Factory Downtime Analysis and Pay Equity Classification

## TLDR

**Project Context**  
Completed through Deloitte Australia’s Data Analytics Virtual Program on Forage, simulating client-facing analytics work.

**Business Goal**  
Identify the biggest sources of assembly-line interruption across global factories and classify gender pay equity by job role and location to support fairer compensation review.

**Primary Stakeholders**  
Daikibo operations leaders reviewing factory downtime, along with internal HR and forensic technology stakeholders reviewing compensation fairness.

**What I Built**
- A Tableau dashboard analyzing industrial IoT telemetry data from 4 factories and 9 machine types
- A calculated downtime measure to quantify unhealthy machine status in 10-minute increments
- A drill-down dashboard showing total downtime by factory and device type
- An Excel-based equality classification analysis labeling roles as Fair, Unfair, or Highly Discriminative

**Key Deliverables**
- Defined the business questions and stakeholder objectives
- Analyzed machine telemetry data to identify downtime concentration
- Built Tableau bar charts and dashboard filter interactions
- Created an equality classification field in Excel using rule-based thresholds
- Delivered visual and tabular outputs to support operational and pay equity review

## Links to Deliverables 

- **Task 1: Tableau Dashboard Screenshots**  
  Dashboard visuals showing downtime by factory and device type.
  - [Final Dashboard Screenshot](task_1_machine_analysis_tableau/final_dashboard_deloitte.png)
  - [Most Down Time Screenshot](task_1_machine_analysis_tableau/most_down_time_deloitte.png)
  - [Unhealthy Calculation Screenshot](task_1_machine_analysis_tableau/unhealthy_calculations.png)

- **Task 2: Equality Table Outputs**  
  Completed equality classification outputs for role-level pay equity review.
  - [Completed Equality Table CSV](task_2_equality_table/Task2_Equality_Table_Completed.csv)
  - [Completed Equality Table PDF](task_2_equality_table/Task2_Equality_Table_Completed_PDF.pdf)

- **Original Data**
  - [Task 1 Original Data](original_data/task1/daikibo-telemetry-data.json.zip)
  - [Task 2 Original Data](original_data/task2/Task%205%20Equality%20Table.xlsx)

**Findings**
- Factory downtime was concentrated unevenly across locations, making it easier to isolate where assembly-line interruptions were most severe
- Tableau filtering made it possible to connect the highest-downtime factory to the device types driving those interruptions
- The Excel classification framework translated raw equality scores into business-friendly categories for review
- The project showed how straightforward rule-based analysis can support both operational diagnostics and pay equity monitoring

**Tools Used**

- Tableau
- Excel

**Why It Matters**

This project shows how analytics can support two very different business problems: operational performance and compensation fairness. It highlights dashboarding, classification logic, and stakeholder-focused analysis in a concise consulting-style case study.

---

## Overview

This project was completed through Deloitte Australia’s Data Analytics Virtual Program on Forage and simulates client-facing work involving operations analysis and forensic technology support.

The project had two separate tasks.

In the first task, I analyzed machine telemetry data from Daikibo’s factories to identify where assembly-line downtime was happening most often and which machine types were driving those interruptions. I used Tableau to build an interactive dashboard that allowed users to filter downtime by factory and examine the device types contributing to operational issues.

In the second task, I worked with compensation data to classify job roles based on an equality score. Using Excel, I assigned each role to a category of Fair, Unfair, or Highly Discriminative so stakeholders could review pay equity concerns in a more structured way.

Together, the project shows how analytics can be used across both operations and people-related business problems.

---

## Core Business Questions

**Task 1: Which factory experienced the most assembly-line downtime, and which device types drove the most interruptions in that location?**

**Task 2: Which roles should be flagged as Fair, Unfair, or Highly Discriminative based on their gender pay equality score?**

These tasks reflect two common consulting-style analytics needs:

- Turning raw operational telemetry into a clear root-cause dashboard
- Turning raw scoring outputs into practical business classifications

---

## Business Context

**Business Objective**  
Support better operational decision-making by identifying downtime concentration, while also supporting a more equitable compensation review process through role-level classification.

---

## Project Structure

### Task 1: Factory Downtime Analysis in Tableau

The first task focused on machine telemetry data from four global factories.

Main work completed:

- Imported telemetry data from JSON format into Tableau
- Created a calculated field called **Unhealthy** with a value of 10 for each unhealthy machine status
- Built a bar chart for **Down Time per Factory**
- Built a second bar chart for **Down Time per Device Type**
- Combined both visuals into a dashboard
- Configured the factory chart as a filter so selecting one factory updated the device-level chart

The goal was to identify which factory had the most downtime and which machine types were causing the most operational interruptions there.

### Task 2: Equality Classification in Excel

The second task focused on compensation equality scores by factory and job role.

Main work completed:

- Reviewed factory, job role, and equality score data
- Created an **Equality Class** column
- Classified each record into one of three categories:
  - **Fair** for scores between -10 and 10
  - **Unfair** for scores below -10 or above 10
  - **Highly Discriminative** for scores below -20 or above 20
- Applied rule-based thresholds to make the classification consistent and easy to review

This helped convert raw scores into a format that stakeholders could interpret more quickly.

---

## Data Sources

- Industrial IoT telemetry data from Daikibo factories
- Equality score table containing:
  - Factory
  - Job Role
  - Equality Score

The telemetry dataset covered four factories:
- Daikibo Factory Meiyo (Tokyo, Japan)
- Daikibo Factory Seiko (Osaka, Japan)
- Daikibo Berlin (Berlin, Germany)
- Daikibo Shenzhen (Shenzhen, China)

The machine dataset included nine device types and machine status readings at 10-minute intervals.

---

## Analysis Approach

### Task 1: Tableau Dashboarding

To measure downtime, I created an **Unhealthy** calculated field with a value of 10 for each unhealthy status. This represented 10 minutes of potential downtime since the previous message.

From there, I built:

- A factory-level downtime comparison
- A device-type downtime comparison
- A dashboard with interactive filtering

This made it easier to move from a high-level operational view to a more detailed root-cause view.

### Task 2: Excel Classification Logic

For the equality analysis, I translated the numeric score into business-friendly categories so the output could be reviewed more efficiently.

The classification logic grouped rows into:

- **Fair**
- **Unfair**
- **Highly Discriminative**

This turned the scoring output into a more practical review table for decision-makers.

---

## Tableau Dashboard Visuals

### Final Dashboard
![Final Dashboard](task_1_machine_analysis_tableau/final_dashboard_deloitte.png)

This dashboard combines downtime by factory and downtime by device type into one interactive view.

---

### Factory with Highest Down Time
![Most Down Time](task_1_machine_analysis_tableau/most_down_time_deloitte.png)

This screenshot highlights the location with the most downtime and the machine types contributing most heavily to interruptions.

---

### Unhealthy Calculation
![Unhealthy Calculations](task_1_machine_analysis_tableau/unhealthy_calculations.png)

This screenshot shows the calculated downtime logic used to convert unhealthy statuses into measurable downtime.

---

## Equality Classification Output

### Completed Equality Table
- [CSV Output](task_2_equality_table/Task2_Equality_Table_Completed.csv)
- [PDF Output](task_2_equality_table/Task2_Equality_Table_Completed_PDF.pdf)

This deliverable translates raw equality scores into clear review categories for each role and factory.

---

## How to Use This Repository

There are three ways to review this project.

### Option A: Review the Tableau Outputs

Open the task 1 image files to review the final dashboard and supporting screenshots.

1. [Final Dashboard Screenshot](task_1_machine_analysis_tableau/final_dashboard_deloitte.png)  
2. [Most Down Time Screenshot](task_1_machine_analysis_tableau/most_down_time_deloitte.png)  
3. [Unhealthy Calculation Screenshot](task_1_machine_analysis_tableau/unhealthy_calculations.png)  

### Option B: Review the Equality Classification Outputs

Open the completed task 2 deliverables.

1. [Completed Equality Table CSV](task_2_equality_table/Task2_Equality_Table_Completed.csv)  
2. [Completed Equality Table PDF](task_2_equality_table/Task2_Equality_Table_Completed_PDF.pdf)  

### Option C: Review the Original Source Files

- [Task 1 Original JSON Data](original_data/task1/daikibo-telemetry-data.json.zip)
- [Task 2 Original Excel File](original_data/task2/Task%205%20Equality%20Table.xlsx)

---

## Deliverables

1. Factory-level downtime comparison  
2. Device-type downtime comparison  
3. Interactive Tableau dashboard with filter behavior  
4. Unhealthy downtime calculation logic  
5. Equality class assignment for each role and factory  
6. Completed CSV and PDF output for pay equity review  
7. Business-friendly visuals and classification outputs for stakeholder interpretation  

---

## Key Takeaways

- Tableau can quickly turn telemetry data into a clear root-cause dashboard for operational review
- Simple calculated measures can make machine-status data more interpretable
- Interactive filtering improves drill-down analysis and stakeholder usability
- Excel classification logic can translate raw scoring into clearer decision categories
- Even smaller analytics tasks can support meaningful decisions in operations and HR contexts

---

## Why This Project Matters

Consulting and analytics work often involves translating raw technical outputs into something stakeholders can understand and act on quickly.

This project brings together operational analysis, dashboarding, classification logic, and business interpretation in a compact client-style case study. It is a good example of how analytics can make technical information more usable for decision-makers.

---

## What I Learned

This project strengthened my ability to:

- Use Tableau to build simple but effective operational dashboards  
- Create calculated fields that turn raw status signals into measurable business metrics  
- Use filtering to improve dashboard interactivity and analysis flow  
- Build structured Excel classifications from numeric scoring logic  
- Translate technical outputs into business-friendly findings for stakeholders  
