# CorrelatedCAMP
## Last Updated May 2025
### Collaborative Project: see report for full author list

The Childhood Asthma Management Program (CAMP) collected data on the long-term effects of three treatments (budesonide, nedocromil, or placebo) on pulmonary function (measured by FEV1) in children 5-12 years old. CAMP followed up with 941 participants for 4.5 years with repeated visits to observe the progression of asthma through puberty. The goal of this project is to use correlated data methods to explore if a treatment is more effective than a placebo in increasing pulmonary function in children. 

The CAMP dataset contains variables pertaining to treatment, age, gender, ethnicity, parental smoking status, and visits and our main outcome being change in forced expiratory volume (FEV_change). To start, we’ll transform the dataset to long format and create our outcome variable by taking the difference of FEV before and after treatment at every visit. With REML, we’ll explore the covariance matrices using LRT for nested models and BIC for non-nested models. Using PROC MIXED with Method = ML, we’ll model on treatment, age, gender, ethnicity, parental smoking, and visits. We will interpret the results of the model and provide the mean change in FEV for each treatment group at each visit. 
