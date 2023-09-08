# Vaccination-and-Epidemic-Spread
In this project, I simulated epidemic spread with and without preventative measures like masking, distancing and the administration of 2-dose vaccines. There are 4 cases considered:

- Natural spread
- Epidemic Spread with basic preventative measures
- Epidemic spread with basic preventative measures and vaccinations—scenario A
- Epidemic spread with basic preventative measures and vaccinations—scenario B

I ran the simulation 500 times for each case and used an ANOVA and a  Tukey HSD test to determine if there is any significant difference between the epidemic durations/infection attack rates between all four models.

I have not modelled any particular disease—the parameters governing the extent and speed of epidemic spread are generated randomly within certain bounds.

\* **Vaccination Scenario A:** prime most individuals with a first dose, and once a sufficient portion of the population is primed, only then rollout the second dose.

\* **Vaccination Scenario B:** prime all individuals with a first dose and follow up with the second dose immediately upon the end of the priming period.

## Conclusions
![Infection Attack Rate and Epidemic Duration by Scenario](/images/boxplots.png)

1. Engaging in preventative behaviours prolongs the duration of an epidemic. This increase is not curbed by using vaccines.

2. In terms of reducing the total number of infected individuals, vaccination strategy A does confer statistically significant additional benefits when used with basic preventative measures. The same cannot be said about vaccination strategy B.

3. Overall, we can conclude that vaccination strategy A is better than vaccination strategy B, but the difference is minute.

## Files

The project code is divided into two files:
- Simulating Vaccine Strategies in an Epidemic.ipynb
	- This file contains the code for the simulation and a exhaustive description of the background, assumptions and mathematics required to understand the simulation.
- Hypothesis Testing.Rmd
	- This file uses the simulated data produced by the simulation. It contains all descriptions and the code pertaining to statistical analysis and hypothesis testing.
 	- A third file 'Hypothesis Testing.md' contains the same content as Hypothesis Testing.Rmd for easy visualization

The simulation output can be found in results.csv

## Planned Improvements

- The `initialize_spread_params` function contains repetitive code. Condense this.
- Add docstrings to simulation functions.
- Separate background and model description into it's own file, away from the simulation code.
- Add background on the statistical tests used and why they were chosen.

