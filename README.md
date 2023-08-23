# Pieris

This repo contains several datafiles, figure outputs, and analysis scripts for the 2022 INTBio Pieris project. 

## North Carolina folder
1. **NC Larval and Realistic Temps** Folder: contains all the data and analysis from summer 2022 with Pieris larvae reared at 16,21,26,30, and 34 degrees, the modeling that followed, and testing this model with April and August temperatures
  1a. **Data** folder: contains all raw and processed datafiles called in scripts
    - Apr1toMay31.csv: Raw datafile from the weather station at RDU Airport on temperatures from April 1, 2020 to May 31, 2020
    - Aug1toAug31.csv: Raw datafile from the weather station at RDU Airport on temperatures from August 1, 2020 to August 31, 2020
    - CleanedRound1.csv: Output datafile from Round1_Cleaning.Rmd which includes empty columns for later calculations
    - CleanedRound2.csv: Datafile for realistic temperature treatments which includes empty columns for later calculations
    - CleanedRound2Old.csv: Datafile for realistic temperature treatments before experiment was finished
    - July1toAug31.csv: Raw datafile from the weather station at RDU Airport on temperatures from July 1, 2020 to August 31, 2020
    - rduairport.csv: Raw datafile from RDU airport with temperature data for 2020
    - Round1_DatesFixed.csv: Datafile that was modified from CleanedRound1.csv which fixed the death dates of larval-pupal intermediates to accurately reflect the day they died. This is the datafile used in analysis.
    - Round1_July5.csv: Datafile with incorrect death dates used during analysis
    - Round1_July6.csv: Datafile with incorrect death dates used during analysis
    - simulated_36_-79_2_d_2022_4_1_5_31_inbetween.csv: Datafile used by our environmental chambers to replicate realistic temperature conditions for April 1-May 31 of 2020
    - simulated_36_-79_2_d_2022_8_1_8_31_inbetween.csv: Datafile used by our environmental chambers to replicate realistic temperature conditions for August 1-August 31 of 2020
    
  1b. **Figures** folder: contains all outputted ggplot figures created by scripts
      - NCAprilTemps.png: Output graph from RealWeatherConditions.Rmd to see what spring temps look like 
      - NCAugustTemps.png: Output graph from RealWeatherConditions.Rmd to see what summer temps look like 
      - DevRateModelFitComparison.png: Comparing the fit of two different models used to fit development rate data for Round 1
      - DevRateModelFitComparison2.png:Comparing the fit of two different models used to fit development rate data for Round 1 (with graphs overlapping)
      - KMAttemptedSurvplot.png: A failed graph to represent survival data from round 1
      - KMAttemptedSurvplot2.png: A failed graph to represent survival data from round 1
      - KMAttemptedSurvplotpupa.png: A graph used to see the surivival of each treatment group to pupation over time
      - NCLarvalMassTime.png:A graph used to see the average mass of Pieris in each treatment group at 4th instar, 5th instar, and pupation compared to the amount of time it took to reach each of those stages
      - WeibullModelFit.png:The Weibull model (line) laid over the development rate of individuals in each treatment group
      - NCLarvalSuccessfulPupations.png: A graph comparing mass as pupation to time to pupation, separated by treatment group (color) and whether or not the individuals pupated successfully (filled vs unfilled circles)
      - NCLarvalSurvival.png: A graph showing a proportion of individuals that survived for each treatment group
      - NCLarvalPupMasstemp.png: A graph showing pupal mass for each treatment group, separated into successful and unsuccessful pupations (larval-pupal intermediates)
      - NCLarvalDevRate.png: A graph showing development rate (1/days to pupation) for each treatment group, separated by successful pupations and unsuccessful pupations (larval-pupal intermediates)
      - DevRateModelWithRealTemps.png: A graph showing the Weibull model for development rate over the actual development rate for each treatment group, along with a histogram showing the amount of times each temperature was reached during the april and august realistic temperature treatments
      - PotentialSpringGraph.png: A graph showing a way that we could have represented a spring in 2020 in a chamber
      - SurvModelFitComparison.png: A graph showing two different models for survival (colored lines) over the actual survival rate for each treatment (black dots)
      
  1c. PossibleThermalConditions.Rmd: shows different thermal scenarios to choose between for the second round temperature regimes 
  1d. RealWeatherConditions.Rmd: creates the file necessary for running the program on the chamber for the April 2020 and August 2020 weather patterns
  1e.  Round1_Analysis.Rmd: codes summary statistics, development rate curves, and Kaplan-Meier curves for the first round data
  1f. Round1_Cleaning.Rmd: cleans the Round 1 data for use in Round1_Analysis.Rmd
  1g. Round2_Analysis.Rmd: codes the summary statistics and observed development times for the second round data (under april and august temperatures)
  1h. Curve_Fitting.Rmd: codes the curve fitting and parameter estimation using the rTPC package
2. **NC Pupal** Folder: contains all data and analysis from Summer 2023 where Pieris larvae were reared at 26+/-5 then switched to temperature treatments upon pupation 
  2a. **Data** folder: contains all raw and processed datafiles called in scripts
  2b.**Figures** folder: contains all outputted ggplot figures created by scripts
3. **NC Egg** Folder: contains all data and analysis from Summer 2023 where Pieris eggs were placed on a metal temperature gradient plate within 24 hours of being laid
  3a. **Data** folder: contains all raw and processed datafiles called in scripts
  3b.**Figures** folder: contains all outputted ggplot figures created by scripts


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
	



