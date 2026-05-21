# Insurance Claims & Policy Analysis Dashboard | Power BI
## Dashboard Link:


https://app.powerbi.com/groups/me/reports/c4fc54a3-4d23-4379-9cfe-c1bb8d2c745b/745bd2c9df60e3702b95?experience=power-bi

## Dashboard Preview

![dashboard](https://github.com/user-attachments/assets/c29a21c6-0d3f-47af-afc1-35e766289814)

## Problem Statement

This project focuses on analyzing insurance policy and claims data to understand:

- Premium and coverage distribution across policy types
- Claim patterns based on age groups
- Active vs inactive policy trends
- Claim settlement and rejection analysis

The dashboard helps insurance stakeholders monitor policy performance, customer demographics, and claim behavior for better business decision-making.

## Data Source & Integration
- Imported raw insurance data into SQL Server Database
- Connected Power BI with SQL Server for centralized data    retrieval and reporting
- Configured scheduled refresh in Power BI Service to ensure - continuous and up-to-date dashboard reporting

   ![sql](https://github.com/user-attachments/assets/448355df-2913-4f50-bec0-2bba91dc93db)

## Dataset Description

The dataset contains insurance-related customer and claims information.

**Key Columns**:
- PolicyNumber – Unique policy identifier
- CustomerID – Customer identification number
- Gender – Male / Female
- Age – Customer age
- PolicyType – Insurance category (Health, Auto, Travel, etc.)
- PolicyStartDate / PolicyEndDate – Policy duration
- PremiumAmount – Premium paid by customer
- CoverageAmount – Total insurance coverage
- ClaimNumber – Claim identifier
- ClaimDate – Date of claim
- ClaimAmount – Claim requested amount
- ClaimStatus – Pending / Settled / Rejected

## Data Cleaning & Transformation (Power Query)

Performed data preprocessing and transformation using Power Query Editor:

- Verified and corrected column data types
- Performed data profiling and transformation
- Cleaned inconsistent and missing values
- Created custom conditional columns for:
  -  Age Group
  - Policy Status (Active/Inactive)

### Conditional Columns Created
Age Group :

If Age <= 24 → Young Adult

If Age <= 60 → Adult

Else → Elder

![cond1](https://github.com/user-attachments/assets/a3132f58-8b45-40fa-a849-9a470a91efb0)

Policy Status : 

If PolicyEndDate <= 10-12-2024 → Inactive

Else → Active

![cond2](https://github.com/user-attachments/assets/a02e74ba-d890-4f3f-91dd-39c6aae8e270)


## Dashboard Features
- KPI Cards
- Total Premium Amount
- Coverage Amount
- Claim Amount

### Visualizations
- Premium Amount by Policy Type
- Active vs Inactive Policies
- Claim Amount by Age Group
- Claim Count by Claim Status
- Policy Type vs Claim Status Matrix

## Key Insights
- Policy Trends
Travel and Health insurance contribute the highest premium amounts
Active policies dominate overall policy distribution

   ![1](https://github.com/user-attachments/assets/68412c49-ed4d-4285-ad3b-1fb20bf01b1f)

- Claim Analysis
Adults generate the highest claim amounts compared to other age groups.
Rejected claims are higher than pending claims, indicating strict validation processes

   ![2](https://github.com/user-attachments/assets/0ef34e2f-8890-41e1-97af-b9814239a830)


   ![3](https://github.com/user-attachments/assets/b2056b46-234f-4870-b058-b6ecd15eae0c)


- Customer Demographics
Male and female customer distribution is nearly equal
Younger adults contribute comparatively lower claim amounts

## Snapshot of Dashboard (Power BI Service):

![powerbi_service](https://github.com/user-attachments/assets/a8b7f7f7-a9f1-4d2d-a857-f96ddbf680fc)

## Scheduled Refresh :

- Implemented scheduled refresh in Power BI Service to automatically update the dataset with the latest loan records  
- Enabled continuous monitoring of key metrics such as default rates, loan distribution, and income segmentation  
- Reduced manual effort by automating data updates, ensuring timely and accurate decision-making  

![sr](https://github.com/user-attachments/assets/1985b96b-13b5-4a77-a027-535399c07f15)

## Tools & Technologies Used
- Power BI Desktop
- Power Query Editor
- DAX
- SQL Server
- Power BI Service
- Data Modeling & Visualization

## Conclusion

This dashboard provides a comprehensive overview of insurance policies, customer demographics, and claim behavior.

The analysis enables stakeholders to:

- Track policy activity
- Monitor claim settlement patterns
- Identify high-performing insurance categories
- Improve decision-making using data-driven insights
