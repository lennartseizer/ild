# What is intensive longitudinal data?  
Intensive longitudinal data, resulting from Ecological Momentary Assessment (EMA), refers to data collected repeatedly over time in ecologically valid settings (e.g. multiple times per day, across days or weeks). Such data allow us to study within-person dynamics, temporal processes, feedback loops, and time-varying associations.
  
## Key characteristics of ILD:
- High-frequency sampling (multiple observations per subject over time)
- Nested/time-series and multilevel structure
- Within-person variation and dynamics are central
- Requires modeling techniques that account for autocorrelation, intraindividual variability, and between-person heterogeneity
  
## Guidelines to model ILD:
- Allow for random effects
- Account for temporal variance as an explicit factor 
- Specify the appropriate number of independent units
- Distinguish the between-person and within-person levels of analysis.
- Choose interpretable zero points for independent variables.


## Required R packages:
```
# List of needed packages
pkgs <- c("simr", "nlme", "lme4", "ggplot2", "cowplot",
"scales", "r2mlm", "tidyr", "parameters", "reshape2",
"HLMdiag", "sjPlot", "dplyr", "forcats", "ggdist", "scales")

# Install any that are missing
install.packages(setdiff(pkgs, rownames(installed.packages())))

# Load them all
invisible(lapply(pkgs, library, character.only = TRUE))
```
