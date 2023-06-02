# Pieris

This repo contains several datafiles, figure outputs, and analysis scripts for the 2022 INTBio Pieris project. 

## North Carolina folder
1. **Data** folder: contains all raw and processed datafiles called in scripts
2. **Figures** folder: contains all outputted ggplot figures created by scripts
3. Curve_Fitting.Rmd: codes the curve fitting and parameter estimation using the rTPC package
4. ProgramCreation.Rmd: codes the output files necessary to run the April and August 2020 temperature regimes on the environmental chambers
5. Round1_Analysis.Rmd: codes summary statistics, development rate curves, and Kaplan-Meier curves for the first round data
6. Round1_Cleaning.Rmd: cleans the Round 1 data for use in Round1_Analysis.Rmd
7. Round2_Analysis.Rmd: codes the summary statistics and observed development times for the second round data 
8. ThermalConditions.Rmd: shows different thermal scenarios to choose between for the second round temperature regimes. 


## Washington folder
This folder contains the data, figures, and analyses for the experiments conducted with Washington state-collected Pieris rapae, sent to UNC by Gwen Shlichta as eggs. We used different fluctuating temperature treatments to investigate how performance differed with temperature. 

1. **DataWA** folder: 
	- WABlock1Dev.csv: Raw datafile for the first experiment run with Washington individuals in Fall 2022, looking at larval development at different temperatures
	- WABlock2Dev.csv: Raw datafile for the second round experiment run with Washington individuals in Fall 2022, looking at larval development at different temperatures
	- WAPupa.csv: Raw datafile for the experiment run with Washington individuals in Fall 2022, looking at pupal development at different temperatures
	- CleanedBlock1.csv: Output of the WA_Cleaning.Rmd script for the first larval experiment, which selects the relevant columns and converts dates to development days
	- CleanedBlock2.csv: Output of the WA_Cleaning.Rmd script for the second larval experiment, which selects the relevant columns and converts dates to development days
	- CleanedPupa.csv: Output of the WA_Cleaning.Rmd script for the pupal experiment, which selects the relevant columns and converts dates to development days

2. **FigsWA** folder: 
	- devrateHtoP.png: development rate curves from hatching to pupation with the first and second block experiments combined, split between individuals that pupated successfully and those that died as larval-pupal intermediates
	



