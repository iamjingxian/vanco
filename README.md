#### vanco
vancomycin dosing; mimic data
working space for vanco work with mornin lab at nus

#### Generate subgroups from test data
* age $\leq$ 65, >65; <br>
* BMI $\leq$ 18.5, > 18.5 and  $\leq$25, >25 and $\leq$ 30, >30; <br>
* eGFR $\leq$ 30, > 30 and $\leq$ 45, > 45 and $\leq$ 60, >60 <br>
    * eGFR: measure of kidney function.
    * mdmr equation at https://www.kidney.org/content/mdrd-study-equation
    * eGFR = 175 x $(S_{Cr})^{-1.154}$ x $(age)^{-0.203}$ x 0.742 [if female] x 1.212 [if black]

#### Re-generate cohort data from MIMIC-IV (v1.0) 
* Access MIMIC-IV v1.0 via physionet on BigQuery; refer to [MIT-LCP repo] (https://github.com/MIT-LCP/mimic-iv/tree/master/buildmimic/bigquery)  
* Refer to sql scripts to generate relations as csv files
* Refer to python scripts to pre-process csv files generated from sql scripts

#### Cohort and subgroup EDA
* Gathering insights from subgroups and cohort

#### [Future] Include the dialysis type (CRRT/intermittent HD) as a feature:
* Refer the MIT-LCP concepts for sql scrpts to extract [rrt](https://github.com/MIT-LCP/mimic-code/blob/main/mimic-iv/concepts/treatment/rrt.sql) and [crrt](https://github.com/MIT-LCP/mimic-code/blob/main/mimic-iv/concepts/treatment/crrt.sqlhttps://github.com/MIT-LCP/mimic-code/blob/main/mimic-iv/concepts/treatment/crrt.sql) relations
