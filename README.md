# Recidivism: Relapse Into Prison 

Recidivism is a criminological term for re-offending. 
This is an analysis of recidivism prediction using the data regarding recidivism by convicted offenders.
Our analysis will highlight which portions of the population of former inmates are at much higher risk of failing to adapt to life outside of prison and help target these populations more effectively. This will benefit taxpayers in the US since there will be a lower prison population to pay for, it will benefit former inmates at higher risk of recidivism since they will receive more help at adapting to life outside of prison, and it will benefit the families and communities of former inmates. 

The file recidivism_final_project.Rmd contains all the outputs and conclusions displayed in the final report and is the only file that should be run which is in the Final Report folder.
The following will output from recidivism_final_project.Rmd:
  1. Divides the data into training, testing, and validation sets
  2. Removes all Female prisoners, remove gender, race, and other unnecessary variables
  3. Preanalysis of variables with bar graph output
  4. Checks for multicollinearity
  5. Creates a function to find the accuracy of each model on the testing data
  6. Creates a plot to look at all statistically significant coefficients (scaled)
  7. Checks accuracy of model
  8. Runs stepwise
  9. Runs lasso regression
  10. Runs ridge regression
  11. Runs Elastic Net regression

Libraries required:
library(tidyverse)
library(lubridate)
library(janitor)
library(car)
library(Rcmdr)
library(caret)
library(corrplot)
library(pROC)
library(kableExtra)
library(broom)
library(gt)  
library(gtsummary)
library(glmnet)
