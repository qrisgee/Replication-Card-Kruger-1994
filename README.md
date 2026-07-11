## Card & Krueger 1994 Replication Project
This repository is a side project I conducted with advisory from the principle investigator of a economic dry lab I participated in during the Winter 2026 and Spring 2026 quarter.
The purpose of this project was to extend and develop transferable skills beyond the responsibilities I held as a research assistant.
At the heart of this project, I was tasked to replicate the 1994 Card-Krueger study that explored the effects of minimum wage raises in New Jersey during 1992 using IPUMS CPS data.
From my findings, I conducted a DiD estimate that yieded a result different from the original study produced in 1994.

## SCRIPTS 
Aside from the intial extraction of the IPUMS data in R, the bulk of data aggregation and compilation was written in Python. I utilized a mix of pandas, seaborn, statsmodel 
and matlibplotlibraries.
* data_cleaning_v4.ipynb
    * In the final script for the data cleaning process, I partitioned the data to focus on New Jersey and Pennsylvania as was done in the original study
    * I introduced 3 dummy variables, NJ_PA, POST_POLICY, and DID_DUMMY that will later be utilized for the visual production and DiD estimation
* visual_production_v2.ipynb
    * Graph 1: a line plot of monthly CPS employment of workers surveyed under the IND1990 641 code: "Eating and drinking places" from 1988 - 1998
    * Graph 2: a point plot of annual CPS average employment of workers surveyed under the IND1990 641 code: "Eating and drinking places" from 1988 - 1998
* post_policy_analysis.ipynb
    * Using the statsmodel library I constructed a weighted least squared model to determine the statistical significance of the observed treatment (The minimum wage increase in
New Jersey in 1992)
## DATA 
* This folder contains the cleaned and aggregated data produced by the data_cleaning_v4.ipynb script after I pulled from original IPUMS 

## OUTPUT
* This folder contains the 2 graphs I produced from the visual_production_v2.ipynb script

## DOCUMENTS
* This folder contains a written document of expected outcomes prior to conducing the DiD estimation and a review of the outcome of my findings. 
