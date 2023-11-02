# POWER-BI-TASK-4

# Introduction:

The ability to derive meaningful insights from data is paramount. This is where Data Analysis Expressions (DAX) functions in Power BI come into play.

The DAX functions serve as powerful tools in Power BI for performing calculations and aggregations and they help to derive meaningful insights and metrics from the dataset.

These DAX functions are used to gain deeper insights, perform advanced analyses, and create customized measures and columns that suit specific business needs. DAX functions provide the flexibility and functionality necessary for robust data modeling and reporting in Power BI.

Problem Statement:
1. Create a measure for the ‘Average age of depositors’
2. Create a new column named ‘Age band’ containing the following:
  ‘Young’ for ages below 30
  ‘Mid Aged’ for ages between 30 and 50
  ‘Old’ for ages above 50
3. Create a measure calculating the total balance for:
  Job: Technician
  Marital: Single and married
4. Create a measure to get the number of depositors on loan

# The screenshots below is showing 1. Average age of depositors = CALCULATE(AVERAGE('bank-full'[age]), FILTER('bank-full','bank-full'[loan]="YES"))

![POWER BI TASK 4 Average age of deposotors](https://github.com/Tonyigba/POWER-BI-TASK-4/assets/143624967/51354438-e11b-406f-a70d-45b05110d089)

![POWER BI TASK4](https://github.com/Tonyigba/POWER-BI-TASK-4/assets/143624967/1313f57c-658a-434b-92a6-408120859340)


# screehoot Below is showing new column "Age Band" = IF('bank-full'[age]<30, "Young", IF('bank-full'[age]<=50, "Mid-Age", "Old"))

![POWER BI TASK 4 AGE BAND](https://github.com/Tonyigba/POWER-BI-TASK-4/assets/143624967/eed394d6-0267-4498-ba1c-5de14f4befa3)


# The screenshot below is showing TOTAL Balance by Job (Technician) = CALCULATE(SUM('bank-full'[balance]), FILTER('bank-full','bank-full'[job]="Technician"))

![POWER BI TASK 4 TOTAL Balance by Job (Technician) = CALCULATE(SUM('bank-full' balance )](https://github.com/Tonyigba/POWER-BI-TASK-4/assets/143624967/14f46bf1-6364-4e68-9ea9-e36d169ea71c)

![POWER BI TASK 4 TOTAL Balance by Job (Technician)](https://github.com/Tonyigba/POWER-BI-TASK-4/assets/143624967/b5ef2ef8-9198-4abe-a126-d52c9594085f)


# The screenshot below is showing Total Balance By Married and Single = CALCULATE(SUM('bank-full'[balance]), FILTER('bank-full','bank-full'[marital] ="Single" ||'bank-full'[marital]="Married"))

![POWER BI TASK 4 Total Balance By Married and Single  2](https://github.com/Tonyigba/POWER-BI-TASK-4/assets/143624967/44bdbd99-1194-4bc1-b335-5b902ccec5a7)

![POWER BI TASK 4 Total Balance By Married and Single](https://github.com/Tonyigba/POWER-BI-TASK-4/assets/143624967/ae04e396-d89c-4023-97d0-6527d012be18)


# NUMBER OF DEPOSITOR ON LOAN = CALCULATE(COUNT('bank-full'[loan]),FILTER('bank-full', 'bank-full'[loan]="YES"))

![POWER BI BASK 4 NUMBER OF DEPOSITOR ON LOAN](https://github.com/Tonyigba/POWER-BI-TASK-4/assets/143624967/5df76705-fdac-427e-8664-1b0ef6b01a78)

![POWER BI BASK 4 NUMBER OF DEPOSITOR ON LOAN  2](https://github.com/Tonyigba/POWER-BI-TASK-4/assets/143624967/065dbda0-4c01-491a-9df6-51c2e4b5afe7)


# Conclusion:
In this analysis, key insights using DAX functions and visualizations were explored.

The average number of depositors on loans was determined using The DAX function. This shows that age is a critical factor in understanding the customer base.

Next, depositors into age bands were categorized using the DAX function. This categorization into "Young," "Mid-Aged," and "Old" based on age ranges provide a clearer insight.

Also, The total balance of individuals working as technicians and those with marital statuses of "Single" or "Married.” were determined. The 'Total Balance by Job (Technician)' and 'Total Balance by Married and Single' highlight the importance of occupation and marital status in financial profiles.

Overall, this analysis shows the power of DAX functions and visualizations in extracting meaningful insights and informed decisions.

