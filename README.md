# Vaccination-and-Epidemic-Spread
In this project, I simulated epidemic spread with and without preventative measures like masking, distancing and vaccinations. There are 4 cases considered:

- Natural spread
- Epidemic Spread with basic preventative measures
- Epidemic spread with basic preventative measures and vaccinations—scenario A
- Epidemic spread with basic preventative measures and vaccinations—scenario B

I ran the simulation 500 times for each case and used an ANOVA F-test and a  Kruskal-Wallis test to determine if there is any significant difference between the epidemic durations/infection attack rates between all four models.

I have not modelled any particular disease—the parameters governing the extent and speed of epidemic spread are generated randomly within certain bounds.

## Conclusions


## Files

The project is divided into two code files:
- Simulating Vaccine Strategies in an Epidemic.ipynb
	- This file contains the code for the simulation and a exhaustive description of the background, assumptions and mathematics required to understand the code.
- Hypothesis Testing.Rmd
	- This file uses the simulated data produced by the simulation. It contains all descriptions and the code pertaining to statistical analysis and hypothesis testing.

The simulation output can be found in results.csv

## Planned Improvements

- The `initialize_spread_params` function contains repetitive code. Condense this.
- Separate background and model description into it's own file, away from the simulation code.
- Add background on the statistical tests used and why they were chosen.

