# rock_crab_fr_dec2018
Rock Crab Feeding Trials - December 2018-January 2019

This is the repository for data associated with functional response measurements of multiple densities of Pacific Rock Crabs on California Mussels. The experiment was conducted in December 2018 and January 2019 by Joseph Curtis and Jeff Childs on behalf of Dr. Adrian Stier. Files are organized and identified as follows:

/analysis: Code for analyzing raw data
Files: avgd_crab_analysis_2019_1_30 - RMD file for analyzing data, with replicates of treatments with identical sets of crabs *averaged*          into one data point
      
       crab_size_parsing_code2019_2_21 - R file for dissociating comma delimited crab size metadata and transforming into long form for
       easier analysis
       
       fit_crab_sym_avg - MATLAB file modified from code by JW White for fitting several types of functional response curves to
       *averaged* trial data, as summarized and generated in the associated *averaged* RMD code (avgd_crab_analysis_2019_1_30 generates
       avg_crab_trial_data_for_ML.csv)
       
       fit_crab_sym_ind - MATLAB file modified from code by JW White for fitting several types of functional response curves to 
       *individual* trial data, as summarized and generated in the associated *averaged* RMD code (avgd_crab_analysis_2019_1_30
       generates ind_crab_trial_data_for_ML.csv)
       
       fr_param - R function for extracting fit parameters from frair package in crab analysis code
       
       ind_crab_analysis_2019_2_15 - RMD file for analyzing data, with replicates of treatments with identical sets of crabs *averaged*          into one data point
       
/analysis/bootstrap: Subset of code used for bootstrapped estimates of functional response fit confidence intervals

Files:  bootstrap_crab_avg - MATLAB file modified from code by JW White for bootstrapping parameters for several functional response 
        curve fits to *averaged* trial data, using data generated in the associated *averaged* RMD code (avgd_crab_analysis_2019_1_30
        generates avg_crab_trial_data_for_ML.csv)

        bootstrap_crab_ind - MATLAB file modified from code by JW White for bootstrapping parameters for several functional response 
        curve fits to *individiaul* trial data, using data generated in the associated *averaged* RMD code (ind_crab_analysis_2019_1_30
        generates ind_crab_trial_data_for_ML.csv)
        
        bootstrap_plotting_2019_4_11 - R code for visualizing bootstrapped confidence intervals generated by bootstrap MATLAB code
        
/analysis/results: Folder for storing products of code, not raw data

        avg_crab_analysis_results_2019_4_4.m - MATLAB data generated and manually saved from fit_crab_sym_avg.m
        
        avg_crab_bootstrap_results_2019_4_p.m - MATLAB data generated and manually saved from bootstrap_crab_avg.m
        
        bootstrap_results_xx_avg.csv - CSV file manually created from associated MATLAB data, with bootstrapped iterations of model
        parameters stored in the associated .m file. xx is a stand in for the functional response equation used in the bootstrapping
        MATLAB code
        
        Extracted_crab_FR_param_from_ML_analysis 2019_4_4.xlsx - Manually extracted and organized parameters for functional response
        curve fits generated in fit_crab_sym_avg and _ind. Averaged and individual results are stored on one sheet each
        
        ind_crab_analysis_results_2019_4_4 - MATLAB data generated and manually saved from fit_crab_sym_ind.m
        
/data: Folder for storing raw or summarized data (results of statistical tests are stored in /analysis/results)

        avg_crab_trial_data_for_ML - Summarized crab functional response trial data (averaged) generated by RMD file avgd_crab_analysis_2019_1_30
        
        crab_feeding_trial_data_dec2018 - Raw trial data and metadata in both .xlsx and .csv formats
        
        crab_size_data_extracted - csv file of crab sizes and identities
        
        crab_video_trial_pilot_datasheet - Working xlsx dataset of preliminary video analysis of crab behavior, not yet ready for import
        into coding languages (JC - 5/3/2019)
        
        ind_crab_trial_data_for_ML - Summarized crab functional response trial data (individual) generated by RMD file ind_crab_analysis_2019_1_30
        
/figures: Folder for storing figures generated by code
