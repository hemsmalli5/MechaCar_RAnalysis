# Analysis of MechaCar Data
 ## Technical Report
<br> ## Background

Resource: mpg testing dataset of 50 potential prototype MechaCars. 

The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance were collected for each vehicle.
MechaCar suspension coil test results from multiple production lots. In this dataset, the weight capacity of multiple suspension coils was tested to determine if the manufacturing process is consistent across lots.
##Observations
###Multi Linear Regression
Multi Linear Regression observations focused on below questions:
1.	Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
2.	Is the slope of the linear model considered to be zero? Why or why not?
3.	Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
In the summary output, each Pr(>|t|) value represents the probability that each coefficient contributes a random amount of variance to the linear model. According to our results, vehicle length and ground clearance (as well as intercept) are statistically unlikely to provide random amounts of variance to the linear model. In other words, the vehicle length and ground clearance have a significant impact on mpg. When an intercept is statistically significant, it means there are other variables and factors that contribute to the variation in mpg that have not been included in our model. These variables may or may not be within our dataset and may still need to be collected or observed.
Despite the number of significant variables, the multiple linear regression model outperformed the simple linear regression. According to the summary output, the r-squared value has increased from 0.37 in the simple linear regression model to 0.71 in our multiple linear regression model and the p-value changed from 2.636e-06 to 5.35e-11.
The slope of the linear model is not considered to be zero. Through this data, we fail to reject the null hypothesis based on the coefficient values, the dependent variable mpg has a linear relationship to few independent variables.

As we see that R2=0.7 and hence 70% of the predictions are correct, so we can determine our predictions are correct.
Fig1: Linear Regression Summary
Inline-style: 
![Linear Regression](https://github.com/hemsmalli5/MechaCar_RAnalysis/blob/master/Summary%20images/Linear%20Regression%20Summary.PNG)

Fig2: Multiple Linear Regression
Inline-style: 
![Multiple Linear Regression](https://github.com/hemsmalli5/MechaCar_RAnalysis/blob/master/Summary%20images/Multiple%20Linear%20Regression%20Summary.png)

Suspension Coil Summary
Suspension Coil manufacturing data summary:<br>
•	Mean: 1499.531<br>
•	Median: 1499.747<br>
•	Variance: 76.234<br>
•	Standard Deviation: 8.731<br>
<br>
 
Fig4: Summary of the Total suspension data by grouping 
Inline-style: 
![Suspension data Summary](https://github.com/hemsmalli5/MechaCar_RAnalysis/blob/master/Summary%20images/Lot%20Summary.png)

Summary Interpretation:
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per inch. Since suspension data variance (76.23) is under 100PSI, we can predict that the current manufacturing data meets the design specifications.

T-Test
Performing the t-test on the suspension coil data determines the suspension coil’s pound-per-inch results are not statistically different from the mean population results of 1,500 pounds per inch. 
		Fig5: T-test on suspension data
The p = 0.51 > 0.05 means we reject the null hypothesis, therefore the average value was not significantly different from the population mean 1500.


