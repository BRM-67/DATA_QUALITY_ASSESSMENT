Welcome to a short documentation of the code repository for our paper:

"A Multi-level Data Quality Assessment of the Empatica EmbracePlus: Signal-, Index- and Condition-Level Validation under Controlled and Naturalistic Conditions."

Thank you for your interest in our work!

This repository consists mainly of 4 distinct folders that hold data and analysis code.

1. The environment set-up:
You will find a .yaml file for the set-up of an Anaconda-type Python environment Run "conda env create -f py_env.yaml" in a python terminal within the directory of the .yaml file. The .ipynb file was created as a Jupyter Notebook for the use in VSCode. This environment is required for the exact reproduction of the analyses. Of course, you can also run the scripts using some other viable Python environment, but might find some differences in your results compared to ours, due to changes in the functionality of the libraries we employed. There is also a .lock file for the set-up of an R environment. Create a .Rprofile with: source("renv/activate.R") Then, create and open an R project in the same folder and install the "renv" package. Then, activate the environment (renv::activate()) and restore all required packages (renv::restore()). We do recommend the use of RStudio for this. The same caveat regarding alternative environments applies here as well.

2. Supplementary Inputs:
This is mostly meta-data that helps for sample characterization and raw physiological data segmentation and alignment.

3. CVA as the first "main" folder with the analyses of cardiovascular data:
First of all, it should be noted that all of the raw data does not live in this repository! Instead it can be found here (https://figshare.com/s/18c60e6ae46f702d1912). In order for all the preprocessing files to run properly, the corresponding folders with the raw data need to be downloaded from figshare and placed in the right directory (i.e., the folders with the CVA prefix belong into the CVA folder).
Do not move any files. Simply drop the folders into the right directory. Apart from that, there is nothing that needs to be kept in mind specifically, expect for the order the scripts need to be run in if you want to recreate all the intermediate preprocessed data as well. 

4. EDA, same game:
Raw data is also found on figshare, but an intermediate preprocessed datafile is also available. The outline of the notebook will point out what can be run without requiring any additional raw data.

In general, the CVA and EDA modules are self-contained and the scripts can be executed independently once the proper environments have been set up. If you have any questions, feedback or want to get in touch for future collaboration, we are happy to hear from you!

Best, 
The authors


