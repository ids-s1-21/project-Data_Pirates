Geographical and societal qualities of countries in the world
================
by Data Pirates

## Summary

The data set that we decided to analyse for this project is called
‘Countries of the world’. The data set has a variety of information
about different aspects of countries in the world between the year 1970
and the year 2017. It is made up of data from the US government
specifically the CIA World Factbook. We decided to rename our variables
using snake case in order make them more accessible to use and to
evaluate.

Our main aim in this project was to research whether there is a
relationship between various geographical, economic and societal
qualities across the different countries. We hypothesized that there
would be at least a weak relationship between quality of life and other
qualities of the country such as economic and physical qualities.
Therefore, we expected that our results would show at least some
correlation between variables which would then in turn support our
hypothesis. In this write up we will develop on the statistical
techniques we used during the course of this project and whether or not
we can conclude that our initial hypothesis is correct.

The first thing we did to answer our research question was to it break
down into 2 components: 1. How strong is the correlation between
economic and societal qualities? 2. How impactful are geographical
qualities on the development and strength of any economy?

In order to answer the first component, we decided to perform some
linear regression in order to explore the relationship between GDP per
capita and death rate, infant mortality and phones per 1000. We saw that
the R^2 value was 0.705. This in turn showed us that there is a fairly
strong relationship between GDP per capita and the death rate + the
infant mortality rate + phones per 1000. Hence, we can determine that
there is a relatively strong relationship between certain economic and
societal qualities.

In order to answer the second component, we first wanted to show the
difference in economic sectors depending on the continent. We used the
agriculture, industry and service variables and saw that America had the
highest value for service but the lowest value for agriculture.
Meanwhile, Africa had the lowest value for service but the highest value
for agriculture. There was also quite a significant difference between
the continent which had the highest value for service (North America)
and the continent which had the lowest value for service (Africa). We
then wanted to find put if there was a relationship between GDP per
Capita and sector. To do this we used the service sector. The output we
generated as a result shows a clear positive relationship between the
proportional size of the service sector and the GDP per capita. We can
look at both graphs to deduce that geographical qualities do have some
sort of an impact not only on the breakdown of a country’s economy, but
also on the strength of that country’s economy. However, when we tried
to analyse how specific geographic qualities (such as arability) affect
the strength of a country’s economy (GDP per capita) our analysis tends
to break down slightly (little to no correlation).

In conclusion, we have used many types of visualisations in order to
show the relationship between various geographical, economic, and
societal qualities in our project. We can now therefore see the results
directly and significantly. Firstly, as our intuition would have us
expect, there is a strong relationship between certain economic and
societal qualities which is shown by visualizing the GDP per capita and
deathrate, infant mortality, phones per 1000. Furthermore, we saw that
there was a quite a strong relationship (at least on a continental
scale) between geographical qualities and economic qualities which is
shown by visualizing different economic sectors against continents, and
then extending our analysis to also show the relationship between
service and GDP.

As a result of all this analysis we can now confirm that our hypothesis
that was that there to be at least a weak relationship between quality
of life and other qualities of the country such as economic and physical
qualities is correct. However, it is difficult to estimate exactly how
strong the relationship between geographical, societal and economic
qualities are due to the mass variability between (and even inside)
every country in the world, at least with a dataset consisting of 20
variables. To more accurately analyse such a complicated question a much
larger dataset would likely be required.

## Presentation

Our slides can be found [here](presentation/presentation.html). And our
presentation can be found here:
(<https://media.ed.ac.uk/media/Ids%20Project/1_nf8ig6y6>)

## Data

Author: CIA Year: 2017 Title: The World Factbook Description: Electronic
Dataset Date viewed and URL: 22nd October 2021
<https://www.kaggle.com/fernandol/countries-of-the-world.>.

## References

<https://www.kaggle.com/fernandol/countries-of-the-world>.
<https://www.cia.gov/library/publications/the-world-factbook/docs/faqs.html>
