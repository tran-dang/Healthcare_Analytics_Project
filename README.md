# Healthcare Wait Time Insights - Project Overview

## The goal of this project is to track the current status of the patient waiting list and analyze historical monthly trends in order to surface recommendations on resource allocation for future references.

## Objectives
- Track current status of patient waiting list
- Analyze historical monthly trend of waiting list in Inpatient & Outpatient categories
- Detailed specialty level & age profile analysis

## Data Scope
The dataset spans from 2018 to 2021 and includes three main categories:
- Inpatient
- Outpatient
- Day Care

The focal points of the analysis are Inpatient and Outpatient.
Additionally, a detailed specialty-level and age profile analysis was conducted.

<!--## Metrics
The analysis focuses on the following key metrics:
- Average & Median Waiting List
- Current Total Waiting List
-->

## Dataset Structure
The dataset consisted of one primary table (combined and appended from 8 tables) and one mapping table, including information about case types, wait time and specialties, as well as age demographics, admission date, and related patient information
<details>
  <summary>More Information</summary>
  
  ### Tables used
  - *Inpatient*: Contains data specific to inpatient waiting lists (Combined from 4 tables).
  - *Outpatient*: Contains data specific to outpatient waiting lists (Combined from 4 tables).
  - *All_data*: Consolidates data from the Inpatient and Outpatient tables, and is used for all visualizations and analyses in this project (Appended from Inpatient and Outpatient).
  - *Mapping_Specialty*: Used for mapping purposes and linking data points geographically.
  The All_data table is the primary dataset used for the analysis, allowing for comprehensive visualizations and insights.
  
</details>
<img width="812" alt="image" src="https://github.com/tran-dang/Healthcare_Analytics_Project/blob/main/assets/Tables.png">



## Insights Summary
#### To evaluate the patient waiting list status, we focused on the following key metrics:
- **Average & Median Waiting List**: Analysis of average and median waiting times for patients.
- **Current Total Waiting List**: Current number of patients on the waiting list.

Key Findings:
#### Average & Median Waiting List
- **Inpatient Category**: Inpatient waiting list trended down by 2.59% between January 31, 2018, and March 31, 2021, but started trending up on August 31, 2020, rising by 0.12% in 7 months.
- **Outpatient Category**: Outpatient waiting list jumped from 515,360 to 541,899 (5.15%) during its steepest incline between November 30, 2018, and February 28, 2019. Outpatient also had the highest average and median waiting list at 80, followed by Day Case at 19 and Inpatient at 12.

#### Current Total Waiting List
- **Inpatient Category**: The list decreased by approximately 4.35%, from 23K to 22K patients, with Paed Orthopaedic showing the highest Avg/Med Wait List at 41.
- **Outpatient Category**: The list increased by approximately 11.72%, from 563K to 629K patients, with Paediatric ENT showing the highest Avg/Med Wait List at 272.

<!--
## Objectives
- Track current status of patient waiting list
- Analyze historical monthly trend of waiting list in Inpatient & Outpatient categories
- Detailed specialty level & age profile analysis -->

## Objectives Analysis
#### 1. Track Current Status of Patient Waiting List:
- Outpatients had the highest average wait list at 80, followed by Day Case at 19 and Inpatient at 12.

#### 2. Analyze Historical Monthly Trend of Waiting List in Inpatient & Outpatient Categories:
- Sum of Total for Day Case (0.64% increase) trended up while Inpatient (2.59% decrease) trended down between January 31, 2018, and March 31, 2021.
- Sum of Total for Inpatient started trending up on August 31, 2020, rising by 0.12% (27) in 7 months.
- Sum of Total for Outpatient jumped from 515,360 to 541,899 during its steepest incline between November 30, 2018, and February 28, 2019.

#### 3. Detailed specialty level & age profile analysis
- #### Specialty Level
  - The average change in patient wait lists among the top 5 specialties was approximately an increase of 13.97%.
  - Accident & Emergency has an abnormally drastic change (100% increase), followed by Paed Cardiology (31.82% decrease).
  - Outpatient dominated most cases, significantly impacting the overall numbers.
  <details>
    <summary>Detailed Information</summary>
    
    - *Accident & Emergency* saw a 100% increase in patients, rising from 0 to 1,111.
    - *Paed Cardiology* had a 31.82% decrease, dropping from 5,166 to 3,522.
    - *Paed Orthopaedic*'s wait list increased by 2.10%, from 4,962 to 5,066.
    - *Paediatric Dermatology*'s wait list grew by 6.01%, from 4,837 to 5,128.
    - *Paediatric ENT*'s wait list decreased by 9.46%, from 7,549 to 6,835.
  </details>

- #### Age Profile
  - Patients aged 16-64 made up 9.38% of the wait list for the 18+ months time band.
  - The 16-64 age group had the highest average wait list at 73.44, followed by 0-15, 0-15, and 65+.

## Recommendations
<!-- This content will not appear in the rendered Markdown 
- **Health for All**: Reallocate budget from Golden Years Security, which has high cost per acquisition, to Health for All campaigns. The second category outperforms across all key metrics, yet we have invested a relatively low amount ($20K) on them.
- **Health Awareness**: Within Health for All campaigns, focus on health awareness-type marketing, and less on product promotion-type campaigns, which had low signup rate and CTR.
- **COVID Campaigns**: Investigate the cause of abnormally high cost per signup for COVID-based campaigns, which had 2 signups that costed over $1K, compared to an average signup cost of $2.2. Consider removing these campaigns altogether.
- **#HealthyLiving**: Decrease investment in this campaign category, which has the highest spend ($46K) but mediocre signup rates compared to Health for All campaigns.


Recommendations-->
- **Inpatient Process Optimization**:
Reallocate resources from elective procedures during peak periods to critical inpatient care, reducing wait times.
Implement a fast-track protocol for acute cases, minimizing non-essential administrative steps.

- **Outpatient Service Enhancement**:
Allocate additional budget to outpatient services, especially during high-demand periods like late 2018 and early 2019.
Expand outpatient consultation capacity by hiring temporary staff during peak months.

- **Specialty-Specific Strategies**:
Increase funding for Accident & Emergency to handle the 100% patient increase effectively.
Reallocate resources from specialties with decreased demand, like Paed Cardiology, to those with increased demand, like Paediatric Dermatology.

- **Targeted Age Group Strategies**:
Prioritize the 16-64 age group with flexible appointment times and a dedicated helpline for quicker triage and referrals.
Develop community outreach programs focusing on preventative care for the 16-64 age group to reduce long-term demand.


## Dashboard
<!--The dashboard can be found in Tableau Public [here](https://public.tableau.com/app/profile/christine3803/viz/RowHealthDashboard/Dashboard). This dashboard enables users to filter by plan, campaign type, and state, and focuses on trends and values in marketing metrics, signup metrics, and claim metrics.

<img width="812" alt="image" src="https://github.com/christinejiang11/rowhealth/assets/56368090/86756aa4-a0d8-44eb-a0d5-c128816f42ac">

Dashboard-->
The dashboard is created in PowerBI, providing interactive visualizations that enable users to filter by category, specialty, and age profile, focusing on trends and values in patient waiting lists.  
The analysis is presented through the following views:
- Summary Page: Provides an overall view of the patient waiting list status.
- Detailed Page: Offers granular analysis at specialty and age profile levels.

View the dashboard [here](https://app.powerbi.com/reportEmbed?reportId=8647c3ea-dc05-495c-be4a-ec658e42fb7f&autoAuth=true&ctid=5cdc5b43-d7be-4caa-8173-729e3b0a62d9) for more insights.


<img width="812" alt="image" src="https://github.com/tran-dang/Healthcare_Analytics_Project/blob/main/assets/SummaryPage.png">

<img width="812" alt="image" src="https://github.com/tran-dang/Healthcare_Analytics_Project/blob/main/assets/DetailedPage.png">
