# Covid and Society

The Git Branch Covidians:

- Tempest Campbell
- Nick Faber
- Teresa Flicek
- Patrick Hudson
- Stuart Yates

### Overview

In the face of the greatest global pandemic since 1919, data scientists have rolled up their sleeves and gotten to work collecting and analyzing data from all corners of the world. For this project, we each picked a topic of interest and looked for datasets to compare with data on Covid-19, mostly from Johns Hopkins. Below are some of our findings.

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

In this portion of the project I looked into COVID-19 key metrics concerning cases, incidence, mortality, and testing data to see if median family income per state, wealthier vs poorer states, to see if an correlations could be attained. My hypothesis entering the research was that median income of a state might play a role in determining how an individual state is preforming overall in terms of previously mentioned health metrics during the pandemic. After completeing some analysis of the data I was able to uncover some correlation between the data and median income. The cumulative rates for mortality, incident rate, and testing rates, all showed either a positive or negative correaltion with state median income. As a general trend the wealthier states had overall lower incident rates and greater levels of testing completed than those on the lower end of the scale. However the mortaility rate stands out in opposition to those values tending to be higher in the wealthy states. This difference was likely the result of many factors, but highlights the socioeconimic complications of the pandemic. With a lack of an overall federal response to the pandemic, the states have been left to bare the burden of the costs of responding to the crisis. As a result the wealthier states tend to be fairing better overall outside of the initial deadly first months of the pandemic. 

### Alcohol Sales

Lorem ipsum...

### Unemployment
#### Is the Colorado Unemployment rate in line with the National Unemplyment rate?
When looking at the unemployment data, I was able to find that the Colorado and National Unemployment data was corelated via a line graph and a scatter plot. I wanted to see if the Colorado unemployment was a good sample of the national unemployment data.

![](/Unemployment/Output/2020_National_and_Colorado_UnemploymentRates.png)

#### Is there a direct correlation with the Colorado Unemployment rate and the National Unemployment Rate?
When looking at the scatter plot for the unemployment data, there was a correlation of the r-value of 0.886 which meant that Colorado was a good sample size for the national data set.

![](/Unemployment/Output/2020 National vs. Colorado Unemployment Rate.png)

#### Is there a correlation between confirmed cases and deaths from COVID-19?

#### Is there a relation between unemplyment rates and covid cases?

