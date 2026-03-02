# When sharks become intentional bycatch

This is a project for [Data Studio](https://journalism.columbia.edu/ms-data-journalism), Spring 2026.

This project analyses the dataset on sharks bycatch from [Worm, Boris et al. (2024)](https://datadryad.org/dataset/doi:10.25349/D9JK6N#readme) to understand what happens to sharks caught "unintentionally" by fishers, and whether their habitats have an influnce on the outcome. 

**Project page:** [sharks-as-bycatch](https://dimuthuattanayake.github.io/sharks-as-bycatch/)

## Methodology

Find in [Analysis](https://github.com/DimuthuAttanayake/sharks-as-bycatch/blob/main/Analysis.ipynb)

### Data collection and cleaning

* Downloaded thedataset from the [Worm, Boris et al. (2024)](https://datadryad.org/dataset/doi:10.25349/D9JK6N#readme)
* Duplicate names for shark species were checked and removed (scalloped hammerhead variations and shortfin mako variations were all made into one label so that there will be one naming standard for these species)
* Dropped rays because I wanted to focus only on sharks
* Names ending in "nei" (not elsewhere included) lump multiple species together, so grouped them into one category and renamed as "other" for clarity.
* Renamed the fates of sharks after being caught by fishers into into three meaningful categories and removed 'discard unknown' because the fate of this category is unknown
* Drop rows with missing values or zero sample size before analysis
* Common name was capitalized


### Analysis

* Because different species had different sample sizes,computed the sample-size-weighted average of 'fate_proportion' within each of the three categories for each species,. 
* Because the three categories of fate comes from different studies, normalized them to 100 percent.
* For chart 2, group species by habitat types and averaged across the categories


### Visualisations

* Chart 1:Created a stacked bar chart showing the percentage of shark bycatch kept onboard without releasing back to the enviorenment
* Chart 2:Created a bar chart showing fate of sharks caught as bycatch from different habitats


## New Skills

* Analysing biodiversity datasets. It's way more complex than I imagined
* Using coding for analysis: because it's so complex I used for Claude for some of it and I have a long way to go before doing this kind of analysis antirely on my own
* Building my first stacked bar chart in Datawrapper
  

## What more would I like to do?

* Learn a better and more accurate methodolody for analysis
* Learn how to combine different datasets together, especially when the data collection methodologies are different. 
* I wanted to use the data set of post release mortality to understand what happens to each of the species once gthey are released by I do not have the technical knowledge needed for that kind of modelling
  

## Contact

Dimuthu Attanayake, [dca2140@columbia.edu](mailto:dca2140@columbia.edu)

