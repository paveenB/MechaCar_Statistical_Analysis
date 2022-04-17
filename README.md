# MechaCar_Statistical_Analysis

## Overview

AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing progress. AutosRUs’ upper management wants to review the production data for insights that may help the manufacturing team.

## Linear Regression to Predict MPG

![This is an image](https://github.com/paveenB/MechaCar_Statistical_Analysis/blob/main/Images/regression.png)

* The most significant variables in our dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. A linear regression model run on these variables against figures for MPG, resulted in p-values of 2.6x10-12 and 5.21x10-8. The intercept was statistically significant.
* The slope of the linear modelis is not zero, as the p-value of 5.35x10-11 is lower than highest level of significance, which means the null hypothesis must be rejected. This means that the relationship between our variables and the miles per gallon is more than random chance.
* Although there are still unconsidered factors, this model does predict the mpg of the MechaCar prototype with some relative effectiveness. The r-squared value of 0.7149 means that the model is 71% accurate.

## Summary Statistics on Suspension Coils

![This is an image](https://github.com/paveenB/MechaCar_Statistical_Analysis/blob/main/Images/total_summary.png)

![This is an image](https://github.com/paveenB/MechaCar_Statistical_Analysis/blob/main/Images/lot_summary.png)

* The overall variance is under 100 psi and meets specifications, there is a problem with one of the individual lots. Lot 3 is well over the acceptable threshold, at 170.28.

## T-Tests on Suspension Coils

![This is an image](https://github.com/paveenB/MechaCar_Statistical_Analysis/blob/main/Images/T-Test.png)

* A review of the results of the T-test for the suspension coils across all manufacturing lots shows that they are not statistically different from the population mean, and the p-value is not low enough (0.0603) for us to reject the null hypothesis.

![This is an image](https://github.com/paveenB/MechaCar_Statistical_Analysis/blob/main/Images/T-Test_Lot1.png)

* A review of the results of the T-test for the suspension coils for Lot 1 shows that they are not statistically different from the population mean, and the p-value is not low enough (1) for us to reject the null hypothesis

![This is an image](https://github.com/paveenB/MechaCar_Statistical_Analysis/blob/main/Images/T-Test_Lot2.png)

* A review of the results of the T-test for the suspension coils for Lot 2 shows that they are not statistically different from the population mean, and the p-value is not low enough (0.6072) for us to reject the null hypothesis.

![This is an image](https://github.com/paveenB/MechaCar_Statistical_Analysis/blob/main/Images/T-Test_Lot3.png)

* A review of the results of the T-test for the suspension coils for Lot 3 shows that they are slightly statistically different from the population mean, and the p-value is just low enough (0.0417) for us to reject the null hypothesis. This lot may be need to be discarded, or at least more closely evaluated.

## Study Design: MechaCar vs Competition

There are many factors that customers take into consideration when evaluating a car purchases. Ridesharing is becoming more important and it is becoming much easier and cheaper to get around using other means. Customers looking to purchase a car are looking for more than just a convenience. They will be looking to buy a car that is an economical means to regularly transport themselves and their items on a reliable, regular basis.

### Metric to test
To narrow down our test, we should evaluate MechaCar's carrying capacity, in cubic inches, in comparison to various competitors' vehicles.

### Null and Alternate Hypothesis
H0: MechaCar prototypes' average carrying capacity is similar to competitor's vehicles in the same vehicle class Ha: MechaCar prototypes' average carrying capacity is statistically above or below that of competitor vehicles.

### Statistical Test Used
The best statistical test for this would be two-sample t-tests.

### What data is needed
We would need to gather cubic space data from the carrying compartments of all MechaCar prototypes, as well as from all major competitor vehicles.
