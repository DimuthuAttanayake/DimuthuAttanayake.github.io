# America's cheese divide: Walmart vs Whole Foods

This is a project for [Data Studio](https://journalism.columbia.edu/ms-data-journalism), Spring 2026.

This project analyses how cheese prices differ between Walmart and Whole Foods, and what that price gap reveals about fat content, consumer demographics, and American food culture. The price and nutritional data comes from [GroceryDB](https://github.com/Barabasi-Lab/GroceryDB), a research database developed by the Barabasi Lab.

## Methodology

### Data collection and cleaning

* Downloaded the GroceryDB dataset from the [Barabasi Lab GitHub repository](https://github.com/Barabasi-Lab/GroceryDB)
* Filtered the dataset to cheese products only (1,621 products across all stores)
* Categorised products into 16 cheese types (Cheddar, Mozzarella, Parmesan, Gouda, etc.) by keyword matching on product names
* Removed uncategorised products and NAs
* Filtered to Walmart and Whole Foods only (880 products)

### Analysis

* Compared **median** prices between Walmart and Whole Foods for each cheese type, calculating dollar and percentage gaps
* Calculated the overall median price difference across all cheese types ($2.53)
* For the fat-per-dollar analysis, filtered out outlier fat values (keeping only 0-50g per 100g) to remove data entry errors
* Computed fat-per-dollar ratios (Total Fat / price) for each product, then took the **median** fat per dollar for each cheese type
* Cross-referenced the price divide with the fat-per-dollar analysis to identify patterns

### Visualisations

* Created a dumbbell chart showing the price gap between Walmart and Whole Foods for each cheese type in Datawrapper
* Created a bar chart showing median fat per dollar by cheese type in Datawrapper
* Embedded both charts into a story page built with the [jsoma fancy-header template](https://jsoma.github.io/page-templates/fancy-header/index.html)

### Notebooks

| File | Description |
|------|-------------|
| `Cheese_comparison.ipynb` | Filters GroceryDB to cheese, categorises by type, compares median prices between Walmart and Whole Foods, calculates price gaps |
| `cheese_priceV_fat.ipynb` | Calculates fat-per-dollar ratios for each cheese type, filters outliers, computes median fat per dollar |
| `GroceryDB_foods.csv` | Source dataset from GroceryDB |

## New Skills

* Using GroceryDB, a research-grade grocery dataset, for the first time to conduct cross-retailer price analysis
* Building interactive Datawrapper charts (dumbbell/range plot and bar chart) and embedding them into a custom story page
* Combining quantitative price analysis with demographic research to build a data-driven narrative
* Using the jsoma fancy-header story template to present the analysis as a visual story with a full-bleed hero image

## What more would I like to do?

* Normalise prices per unit weight (e.g., per 100g) rather than per package to make comparisons more precise
* Add a third retailer (e.g., Target or Aldi) to see where they fall on the price spectrum
* Build an interactive map showing Walmart vs Whole Foods store locations overlaid with income data by census tract
* Analyse protein-per-dollar alongside fat-per-dollar to give a fuller nutritional picture
* Investigate whether organic vs conventional labelling explains the price gap within the same cheese type

## Contact

Dimuthu Attanayake, [dca2140@columbia.edu](mailto:dca2140@columbia.edu)
