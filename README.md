# MechaCar_Statistical_Analysis

## 1.Linear Regression to Predict MPG
I used multiple linear regression to observe multiple independent variables to account for parts of the total variance observed in the dependent variable(mpg).
In multiple linear regression model.
statistical metrics obtained as shown in image below 
![LinearRegressionMatricsPredict MPG.png](https://github.com/deepayogesh/MechaCar_Statistical_Analysis/blob/1f2b858f9dda1593fee314434098d5ec0ccb8ef5/img/LinearRegressionMatricsPredict%20MPG.png)

(1)Which variables/coefficients provided a non-random amount of variance to the mpg values in the data set?
Pr(>|t|) value represents the probability that each coefficient contributes a random amount of variance to the linear model.
vehicle_length,Intercept and ground_clearance these variables has non random amount of variance to mpg.

(2)Is the slope of the linear model considered to be zero? Why or why not?
Slope of the linear model is not considered to zero as we can see the multiple R-squared value is not 0 
3-Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
a simple linear regression model may be more appropriate than a multiple linear regression model. However, the amount of information that can be obtained and analyzed will be far greater using a multiple linear regression.

## 2.Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
Total summary of the data frame
![total_sumary.png](https://github.com/deepayogesh/MechaCar_Statistical_Analysis/blob/1f2b858f9dda1593fee314434098d5ec0ccb8ef5/img/total_sumary.png)
Observing total summary we can see the variance of suspension coils do not exceed 100 pounds per square. 

On observing this summary on each lot
![lot_sumary.png](https://github.com/deepayogesh/MechaCar_Statistical_Analysis/blob/1f2b858f9dda1593fee314434098d5ec0ccb8ef5/img/lot_sumary.png)

We can see the variance of lot 3 exceed the limit. 

## 3.T-Tests on Suspension Coils
One sample T-test on Metrics seen as below (the entire data frame)
![One-sample T-test.png](https://github.com/deepayogesh/MechaCar_Statistical_Analysis/blob/1f2b858f9dda1593fee314434098d5ec0ccb8ef5/img/One-sample%20T-test.png)

The result shows the p-value equals to 1 and our assumed significance level is 0.05.
our calculated p-value is larger than our significance level, we would say that we do not have sufficient evidence to reject our null hypothesis, and therefore we fail to reject our null hypothesis.

Two- Sample test with population2 (LOT2) and population 3(LOT3) 
![2sampleTest-23.png](https://github.com/deepayogesh/MechaCar_Statistical_Analysis/blob/1f2b858f9dda1593fee314434098d5ec0ccb8ef5/img/2sampleTest-23.png)

The result shows the p-value= 0.03584 smaller than our assumed significance level 0.05. Our calculated p-value is smaller than our significance level, we can  state that there is sufficient statistical evidence that our null hypothesis is not true, and therefore we would reject our null hypothesis.

## 4.Study Design: MechaCar vs Competition.
Short description of a statistical study that can quantify how the MechaCar performs against the competition. 

Two-sample t-tests are flexible and can be used  to compare two samples, each from a different population.
The biggest difference between paired and unpaired t-tests is how the means are calculated.
In an unpaired t-test, the means are calculated by adding up all observations in a data set, and dividing by the number of data points. In a paired t-test, the means are determined from the difference between each paired observation. As a result of the new mean calculations, our paired t-test hypotheses will be slightly different.

What metric or metrics are you going to test?
Lets observe the matric for one sample t-test here

![One-sample T-test.png](https://github.com/deepayogesh/MechaCar_Statistical_Analysis/blob/1f2b858f9dda1593fee314434098d5ec0ccb8ef5/img/One-sample%20T-test.png) 

We can see the mean  value is 3.175732
Lets observerd the paired matrics for population1  (Lot1) and  Population3 (Lot3) results 

![pairedt-testin13](https://github.com/deepayogesh/MechaCar_Statistical_Analysis/blob/1f2b858f9dda1593fee314434098d5ec0ccb8ef5/img/pairedt-testin13.png)

We can see the mean value changed to 7.6022172 and p-value is 0.04347 below assumed significant level of of 0.05 percent.
Therefore, we would state that there is not enough evidence to reject the null hypothesis and there is no overall difference in PSI between suspension coils in different lot. 

What is the null hypothesis or alternative hypothesis?
Null hypothesis 
H0 : There is no statistical difference between the two observed sample means. 
Alternative hypothesis means 
Ha : There is a statistical difference between the two observed sample means.

What statistical test would you use to test the hypothesis? And why?
one Sample t-test or two sample t-test can be used to test the hypothesis. 

What data is needed to run the statistical test?
Data need to satisfy following assumptions to run statistical test
(a)We need numerical and continuous data.
(b)We need sample data selected randomly from its population 
(c)Input data needs to be normally distributed 
(d)Sample size should be reasonably large.
(e)Variance of the input data should be similar. 




