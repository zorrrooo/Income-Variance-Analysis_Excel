# Employee Income Variance Analysis for Payroll Anomaly Detection





## Project Overview

This project analyzes employee income data by comparing base pay with current pay to identify compensation anomalies and inconsistencies. The model helps detect unexpected pay variations, improves payroll transparency, and supports financial oversight through structured variance analysis

## Business Problem

Organizations managing large payroll datasets may experience inconsistencies in employee compensation due to system errors, delayed updates, or incorrect adjustments. Without a structured monitoring framework, these anomalies may remain undetected. This project aims to develop a simple analytical framework to detect unusual differences between employees’ base pay and current/ actual pay

## Data Description

A syntehtic data has been created for the analysis purpose using ChatGPT. The dataset includes 3000 employees compensation information such as:

a. Applicant/ Employee ID 

b. Application Date

c. First Name

d. Last Name 

e. Gender

f. State

g. Education Level

h. Experience

i. Job Title

j. Pay

k. Other variables in raw data were not considered including city, zip code, country, address, date of birth etc. 

## Analytical Approach

a. The analysis compares base pay against current pay and calculates the percentage deviation to identify anomalies

b. Employees with unusually high positive or negative variance are flagged for further review

c. further review includes working on ERPs to check if employees were awarded some incentive due to extra effort in the pay period or maybe a temporary/ permanent pay increase

## Tools Used

ChatGPT:

a. Synthetic Data - prompted to create a sample employees dataset for a typical organization

Microsoft Excel: 

a. Pivot Tables - data summary statistics (sum, count, average, sub-classes, standard deviation) to get familiarize with the data

b. VLOOKUP - applied on Base Pay column in the Variance tab 

c. Conditional Formatting - anamoly confirmation highlighted with a "Yes"

=IF(J2<>K2, "Yes", "No")

d. Variance Calculations - shows the exact increase or decrease from the actual pay

=VLOOKUP(A2,'Base Pay'!$A$1:$L$3001, 12, 0)

e. Dashboard - shows the summary statistics, gender-wise pay distribution, and variance confirmation visual

## Key Features of the Model

a. Automated variance calculation between base pay and current pay 

b. Conditional formatting to highlight and yield "Yes" abnormal pay changes

c. Summary dashboard for payroll review 

d. Easy monthly update for ongoing monitoring

## Key Insights

The analysis can highlight:

a. Unusual compensation adjustments 

b. Potential payroll data entry errors 

c. Employees with sudden pay increases or decreases

## Business Impact

The model improves payroll monitoring by enabling faster detection of compensation anomalies and reducing manual verification efforts. It provides a structured approach for reviewing employee pay adjustments and strengthens internal financial controls through

  a. Enhanced payroll transparency
  
  b. Improves accuracy
  
  c. Enables faster identification of compensation anomalies.

## Future Improvements

Potential enhancements include:


a. A synthetic data could be created and entire end-to-end process could be ran using AI tools to avoid manual work - Mostly.ai (synthetic data) and Julius.ai (analysis)

b. Automated anomaly detection using statistical thresholds

c. Integration with payroll databases

d. Visualization using Power BI or Tableau

e. Time-series analysis of compensation trends 

f. Regression analysis to find the casuality between important variables impacting the pay rate

g. Can be applied at the organization level to track and compare departments and performance


## Limitations
Due to large dataset having 3000 employees, 18 vairables and several tabs, the analysis file cannot be viewed/ downloaded in GitHub. Screenshots and formulas shared above to off-set this challenge 
