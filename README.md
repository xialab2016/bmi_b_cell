# Effects of BMI on early B-cell repopulation and an exploration of the clinical impact of early B-cell repopulation

## Background and Objective

Early B-cell repopulation is a phenomenon observed in patients with multiple sclerosis (pwMS) being treated with B-cell depleting therapies, and current research is mixed regarding both potential predictors and potential clinical implications. The aim of this study is to better understand the relationship between BMI and early B-cell repopulation in pwMS, as well as to better understand clinical implications of early B-cell repopulation in terms of MS related disability.

## Methods

This was a multi-center observational, retrospective study including 293 pwMS, all of which were infused at least once with a B-cell depleting therapy. Clinical data, demographic information, and outcomes measuring MS-related disability were extracted and used in analysis. Linear and logistic regression models were used to generate primary analysis results.

## Data analysis

### Repopulation analysis

Run all_repop_new.rmd. Ensure that Database.csv and bmi_bcell_raw.csv are updated. This should result in the output file all_repop.csv.

### Rerunning BMI vs. Repopulation 

Open bmi_bcell_bmi_analysis.rmd. The EDSS code can be found after line 500. 
EDSS scores were derived based on the following AR-EDSS tool: https://aliman.shinyapps.io/nARMSS/

### PDDS Confirmed/Sustained Disability

Run PDDS_Query.rmd. This should result in the output file pdds_all.csv.

#### Confirmed Disability

Run confirmed_disability_pdds.rmd. This should result in the output file conf_disability_output.csv.

Run BMI Bcell confirmed disability. Read in "conf_disability_output.csv" at line 46.

#### Sustained Disability

Run PDDS Sustained Disability.rmd. This should result in the output file df_sustain.csv.

Run BMI Bcell confirmed disability.rmd. Read in "df_sustain.csv" at line 46.

### Rerunning Functional Testing

Download updated version of PROMOTE Database. Open bmi_bcell_functional_testing.rmd and run from line 42, univariate and multivariate analysis code is toward the end. Update the appropriate covariates as necessary.

### Rerunning OCT

Open oct_cleaning_query.rmd and run with the updated PROMOTE Database file, final output should be called ‘oct_bmi.csv’. 

Open oct_bmi_bcell.rmd and run the code starting at line 345 where you import "oct_bmi.csv". 







