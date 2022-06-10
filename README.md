# MechaCar_Statistical_Analysis


## Linear Regression to Predict MPG

![deliverable_1](https://user-images.githubusercontent.com/100378319/173136964-f6dd3c24-d889-4292-9fe2-3541c73b5dab.png)

After performing "summary" for the MechaCar_lm:

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

vehicle_length, spoiler_angle, and AWD are also providing a non-random amount of variance to the mpg values, their Pr(>|t|) are 0.0776, 0.3069, and 0.1852 respectively.

2. Is the slope of the linear model considered to be zero? Why or why not?
The slope of the linear module is not considered to be zero because the p-value( 5.08e-08 ) of intercept is less than 0.05.

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

Yes, based on the R-squared value (0.7149) which is 71% of a mpg prediction will be correct while using this linear model.


## Summary Statistics on Suspension Coils

![total_summary](https://user-images.githubusercontent.com/100378319/173136989-4c2274cf-4206-4d8c-8242-b0b2d2312a81.png)

In total_Summary, we can see the variance of 3 lots is 62.29 which is less than 100 pounds requirement.

![lot_summary_1](https://user-images.githubusercontent.com/100378319/173137002-a28ebfbe-5bee-4417-810a-2cda02a32381.png)

In lot_summary, the variance for lot 1 and lot 2 are 0.98 and 7.47 which meet the standard, however for Lot 3, the variance is 170.28 PSI which is much over the requirement, therefore Lot 3 does not meet the maximum variance requirement.

## T-Tests on Suspension Coils

![t_test_all](https://user-images.githubusercontent.com/100378319/173137064-46149d05-852a-45f4-9a57-4e60b02162e4.png)

For the t-test for all lots, the p-value is 0.06 which is not less than the significance level of 0.05, therefore the sample mean is not statistically different from the population mean of 1500 PSI. We will not reject the null hypothesis.

![t_test_3](https://user-images.githubusercontent.com/100378319/173137079-03344eb4-0bfb-41f0-9d9a-f7f123809503.png)

For the individual lot test: p-value of Lot 1 and Lot 2 are respectively 1 and 0.6072, the sample is not statistically different from the population mean of 1500, there is not sufficient evidence to reject the null hypothesis.

However, for the p-value of Lot 3 is 0.04168. It is statistically different from the population mean. We will reject the null hypothesis.

## Study Design: MechaCar vs Competition

There are so many factors for a customer to consider purchasing a car: selling price, safety issue, performance, the reputation of the brand, etc. To have a comprehensive comparison we will need to have a deep analysis, however I will pick one of the most important factors for the analysis - Performance.

Selling price is important, but performance is also very important to customers. We will perform some performance test with different variance.

- What metric or metrics are you going to test?

The metrics I am going to test are:

Fuel economy (mpg): dependent Variable

Top speed: Independent Variable

Torque: Independent Variable

Annual maintenance cost: Independent Variable

Weight: Independent Variable

Braking distance: Independent Variable

- What is the null hypothesis or alternative hypothesis?

• Null Hypothesis (Ho): Based on overall performance, MechaCar's mpg is outperform than competitors.

• Alternative Hypothesis (Ha): Based on overall performance, MechaCar's mpg is underperform than competitors.

- What statistical test would you use to test the hypothesis? And why?

I would perform Multiple Linear regression since there are more than two independent variables. We can make a prediction about the mpg based on the other independent variables. We would also be able to determine if the independent variables are correlated with each other as well as the relationship between each other.

- What data is needed to run the statistical test?

In order to run the statistical test, we would need the Fuel economy(mpg), Top speed, Torque, Annual maintenance cost, Weight, and Braking distance from both MechaCar and the competitors
