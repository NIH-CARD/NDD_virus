# NDD_virus
Repository for pilot analyses exploring NDD and viral associations in a hypothesis free manner.

**FinnGen_Search_Terms**

Creates csv file of FinnGen viral endpoints that have data for six neurodegenerative diseases (AD, ALS, dementia, MS, PD, and vascular dementia); do this step before running Finn_Gen_Virus_FDR or Finn_Gen_Virus_ALL_lags

**Finn_Gen_Virus_FDR**

Adds FDR correction to viral exposure before NDD at lag 0; can also use to get viral exposure at all lags before NDD

**Finn_Gen_Virus_ALL_lags**

Selects viral endpoint/NDD pairs that have data for both viral exposure before NDD and viral exposure after NDD diagnosis; adds FDR correction

**UKB_Virus_FDR**

Recreates the viral endpoints used in FinnGen using ICD10 codes; uses logistic regression to predict the effect of viral exposure on each NDD. Covariates include age at enrollment, genetically determined sex, and Townsend deprivation index. Adds FDR correction.

**Virus_NDD_Figure**

Creates figure showing hazard ratio lags for replicated associations between viral exposures and NDDs. 

**PRS_UKB_Prep**

Calculates the PRS for activity and diet; do this step before running PRS_UKB_Virus_FDR

**PRS_UKB_Virus_FDR**

Same as UKB_Virus_FDR above except that it also includes the PRS calculated in PRS_UKB_Prep as covariates
