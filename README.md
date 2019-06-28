# Replacing Scientists by Machines - data preparation and analysis
Jupyter notebooks containing data preparation and data analysis for my bachelor's thesis: Replacing Scientists by Machines.

# EPPI-Reviewer and Automated Systematic review
Bench-marking simulations were run on these two software products, and their results are in the corresponding xlsx and csv files.

# Explanation of the folders and files

## Dataset prep - folder

### Dataset inspection without duplicates.ipynb - file
Inspection of processed data by https://github.com/msdslab/automated-systematic-review-datasets

### Dataset prep for simulations.ipynb - file
Further processing of the dataset to allow for the running of simulations. For scientific validity, this exact same dataset was used for both EPPI-Reviewer and Automated Systematic Review

### PTSD_VandeSchoot_18.csv - file
Labelled CSV file containing the data of the initial search of the mentioned paper by Rens van de Schoot.

### simulationdata.csv - file
Output of "Dataset prep for simulations.ipynb notebook", and contains the dataset that was ultimately used for the simulations.

### Original - folder
Contains the files schoot-lgmm-ptsd-included-2.csv and schoot-lgmm-ptsd-initial.csv, containing the inclusions and the results of the initial search respectively. The file with the initial search still contains some duplicates, and was used as the basis for running the simulations on EPPI-Reviewer and Automated Systematic Review.

## EPPI and ASR analysis - folder

### Analysis EPPI and ASR.ipynb - file
Jupyter notebook (python) file with analysis of the simulation results using pandas and NumPy. Analysis was performed on three different metrics: the WSS@95%, WSS@100% and the RRF@10% metrics. Furthermore, averages, standard deviations, minimum values and maximum values were retrieved for scientifically valid comparisons. Ultimately outputs two plots that were also used in the final bachelor's thesis. 

### asrdf.csv - file
File containing the results from Automated Systematic Review when retraining the model after each 10 abstracts. The data was sampled in the same way, so each index i corresponds to the ((i+1) * 10)th amount of abstracts screened.

### eppiresults.xlsx - file
Results from the simulations that were ran on EPPI-Reviewer
