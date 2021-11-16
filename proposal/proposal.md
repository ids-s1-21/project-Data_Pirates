Project proposal
================
Data Pirates

``` r
library(tidyverse)
library(broom)
library(here)
```

## 1. Introduction

The dataset that we have decided to analyse for this project is called
‘Countries of the world’.

In this project we aim to research the relationships between various
geographical and societal qualities across the different countries.

There are 20 variables in this dataset, which include: `country`,
`region`, `population`, `area`, `pop_density`, `coastline`,
`net_migration`, `infant_mortality`, `GDP`, `literacy`, `phones`,
`arable`, `crops`, `other`, `climate`, `birthrate`, `deathrate`,
`agriculture`, `industry` and `service`.

Of these 20 variables: `country` and `region` are string variables,
`area`, `pop_density` and `GDP` are integer variables, and the rest are
decimal variables.

Each observation represents different physical/geographical and societal
attributes of each country in the dataset. There are 227 observations in
total.

This data set has information about the different countries between 1970
and 2017. It is made up of data from the US government specifically the
CIA World Factbook. We obtained this data from
<https://www.kaggle.com/fernandol/countries-of-the-world>.

## 2. Data

    ## Rows: 227 Columns: 20

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr  (2): Country, Region
    ## dbl (18): Population, Area (sq. mi.), Pop. Density (per sq. mi.), Coastline ...

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

Uploaded the dataset in data folder. There is a total of 227
observations and 20 variables in this dataset.

## 3. Data analysis plan

Our outcome is quality of life, and this will be based on a few
variables - `literacy`, `GDP`, `infant_mortality`, `death_rate`… Our
predictor will also be based on a few seperate variables -
`net_migration`, `pop_ density`, `climate`, `arable`…

We should expect to use a variety of inferential statistical methods,
mainly correlation and regression analysis.

Our hypothesized answer is that there would be at least a weak relation
between quality of life and other qualities of the country, therefore
results that show some correlation between variables would support our
hypothesis.

``` r
intro_statistics_1 <- Countries_of_the_world %>%
  select(region, infant_mortality, GDP) %>%
  arrange(desc(GDP))
intro_statistics_1
```

    ## # A tibble: 227 × 3
    ##    region              infant_mortality   GDP
    ##    <chr>                          <dbl> <dbl>
    ##  1 WESTERN EUROPE                  4.81 55100
    ##  2 WESTERN EUROPE                  3.7  37800
    ##  3 NORTHERN AMERICA                6.5  37800
    ##  4 NORTHERN AMERICA                8.53 36000
    ##  5 LATIN AMER. & CARIB             8.19 35000
    ##  6 WESTERN EUROPE                  5.73 34600
    ##  7 WESTERN EUROPE                  4.39 32700
    ##  8 WESTERN EUROPE                  4.56 31100
    ##  9 WESTERN EUROPE                  3.31 30900
    ## 10 WESTERN EUROPE                  4.66 30000
    ## # … with 217 more rows

``` r
Countries_of_the_world %>%
  ggplot(aes(x = GDP, y = infant_mortality)) +
  geom_point() + 
  labs(
    x = "GDP Per Capita",
    y = "Infant Mortality"
  )
```

    ## Warning: Removed 3 rows containing missing values (geom_point).

![](proposal_files/figure-gfm/intro-statistics-1.png)<!-- -->

As shown in the graph usually as the GDP Per Capita goes up the infant
mortality goes down.
