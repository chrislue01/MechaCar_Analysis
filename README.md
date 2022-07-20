# MechaCar_Analysis

Background
A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:

Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
Run t-tests to determine if the manufacturing lots are statistically different from the mean population
Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.


Deliverable 1: Linear Regression to Predict MPG
Deliverable 1 Instructions
The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using your knowledge of R, you’ll design a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. Then, you’ll write a short interpretation of the multiple linear regression results in the README.md.


![linear_regression_div1](https://user-images.githubusercontent.com/99819387/179877908-58743ba3-4b0e-465c-b1c3-953b4c21196f.png)

From the above output we can see that:

1 The vehicle length, and vehicle ground clearance are likely to provide non-random amounts of variance to the model.

2 The p-Value for this model, p-Value: 5.35e-11, is much smaller than the assumed significance level of 0.05%.

3 This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. 



Deliverable 2:
Your total_summary dataframe should look like this:
![Div2](https://user-images.githubusercontent.com/99819387/179878431-0ee0e9e6-4c89-4488-9e5b-072459a781da.png)

Write an RScript that creates a lot_summary dataframe using the group_by() and the summarize() functions to group each manufacturing lot by the mean, median, variance, and standard deviation of the suspension coil’s PSI column. Your lot_summary dataframe should look like this:
![Div2 2](https://user-images.githubusercontent.com/99819387/179878556-4f755219-ff2e-4526-acaf-302730f2e13a.png)


Results:
![total_lot_summary_div2](https://user-images.githubusercontent.com/99819387/179878669-1d1a4cbc-12f2-4c0a-83c5-25ef417a2be2.png)

![manufactoring_lot_summary_Div2](https://user-images.githubusercontent.com/99819387/179878686-436b29c3-96a4-4741-a0eb-7cb00bdb1578.png)

This boxplot shows the differences between the lots:

<img width="543" alt="boxplot2_div2" src="https://user-images.githubusercontent.com/99819387/179878844-76533407-addf-4b1f-ac7a-cd7f901dd8af.png">

Deliverable 3:
t-Tests on Suspension Coils

REsults:
<img width="445" alt="Div3" src="https://user-images.githubusercontent.com/99819387/179878935-dc13539f-c35a-4fa3-9921-ba9bd4a63d4a.png">

<img width="429" alt="Div3 2" src="https://user-images.githubusercontent.com/99819387/179878946-d9ebe6fb-2a64-4235-ab38-92c128cd5877.png">

Deliverable 4:
Study Design: MechaCar vs Competition
Deliverable Requirements:
Using your knowledge of R, design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

The statistical study design has the following:

A metric to be tested is mentioned
A null hypothesis or an alternative hypothesis is described
A statistical test is described to test the hypothesis
This study would involve collecting data on MechaCar and its comparable models across several different manufacturers over the last 3 years.

What are the competitions' comparable models,
Which cars will MechaCar be competing with head-to-head? which cars will be included in the study?
Which factors will look at the study to determine the relevant to selling price?
Metrics
Collecting data for comparable models across all major manufacturers for past 3 years for the following metrics:

Safety Feature Rating: Independent Variable
Current Price (Selling): Dependent Variable
Drive Package : Independent Variable
Engine (Electric, Hybrid, Gasoline / Conventional): Independent Variable
Resale Value: Independent Variable
Average Annual Cost of ownership (Maintenance): Independent Variable
MPG (Gasoline Efficiency): Independent Variable
Hypothesis: Null and Alternative
After determining which factors are key for the MechaCar's genre:

Null Hypothesis (Ho): MechaCar is priced correctly based on its performance of key factors for its genre.
Alternative Hypothesis (Ha): MechaCar is NOT priced correctly based on performance of key factors for its genre.


