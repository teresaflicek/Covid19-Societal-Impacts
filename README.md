# Covid and Society

The Branch Covidians:

- Tempest Campbell
- Nick Faber
- Teresa Flicek
- Patrick Hudson
- Stuart Yates

### Overview

Lorem ipsum...

### Obesity and Food Deserts

Lorem ipsum...

### Faith in Science

What kinds of impacts does people's trust in scientists and health professionals have on prevalance of Covid-19 in their communities?

For this analysis, I mainly looked at 2 surveys:

- Yale data on climate change beliefs to measure trust in science
- NY Times data on estimated mask usage to measure trust in health authorities
- Vaccination data from the CDC

In general, the correlations I was looking for were very weak:

![global warming by state](Science/output/cases-vs-gw-by-state.png)

R-squared: 0.066

![mask use by county](Science/output/cases-vs-masks-by-county.png)

R-squared: 0.022

I wasn't expecting much more to be honest. There are so many other factors affecting exposure, and the data from initial hotspots like New York certainly muddies the waters. (I attempted some outlier scrubbing, but that only helped a little bit.) Perhaps in a year it will have regressed to the mean somewhat, but at this stage of the pandemic, there's too much signal to noise. Null hypothesis not disproved.

As for vaccines, the CDC data is available as a DAT file containing a lot of numbers. They supply you with some R scripts to turn it into an RData file, and a PDF descibing all the columns. It seemed excessive, but I went ahead and set up an R environment, managed to run the scripts, and used a package called Rio to output a CSV. Unfortunately, the data wasn't what I thought it was, so I ended up abandoning that analsysis.

### Income

Lorem ipsum...

### Alcohol Sales

Lorem ipsum...

### Unemployment

Lorem ipsum

## Conclusions

Lorem ipsum
