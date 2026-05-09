# The forests America lost, and found again

An interactive D3 chart that ranks every contiguous U.S. state by how much its forest cover has grown or shrunk since 1945.

In 70 years, the United States traded tens of millions of acres of farmland and forest for cities, parks and ranches. But the trades did not happen everywhere. New York, Alabama and Georgia grew their forests back as old farms were abandoned. California and Texas lost their forests to range and suburb. The chart lets you watch every state make its own swap, one census at a time.

## Files

- `state-rankings.html`, the chart page (D3 v7, served as a static file).
- `mlu.js`, pre-processed state-by-year acreage data (USDA ERS Major Land Uses, 48 contiguous states, 1945 through 2017).

## Data source

USDA Economic Research Service, Major Land Uses inventory:
[https://www.ers.usda.gov/data-products/major-land-uses](https://www.ers.usda.gov/data-products/major-land-uses)

The `mlu.js` file is a pre-processed slice of the ERS state-year-wide CSV. Six categories are kept (forest, grazed forest, ungrazed forest, cropland, urban, grassland and pasture, plus total land), reconciled across 16 census years from 1945 to 2017. Forest sub-fields and "forest as a share of state" are derived in the chart's JavaScript.

## How the chart works

- One row per state, sorted by percent change in forest cover since 1945.
- Green rows mean the state has more of that field today than it did in 1945, brown means less. Deeper shades mark a swing of at least 50 percent.
- Year slider scrolls through the 16 USDA censuses (1945, 1949, 1954, 1959, 1964, 1969, 1974, 1978, 1982, 1987, 1992, 1997, 2002, 2007, 2012, 2017).
- Forest field switches between total forest, grazed forest, ungrazed forest, and forest as a share of state.
- Right-side panel shows the U.S. national figure and the states with the biggest changes since 1945.

## Built with

- [D3.js v7](https://d3js.org/) for the lollipop chart, transitions, force layout and SVG export.
- Plain HTML, CSS and vanilla JavaScript. No build step.
- Built with the assistance of Anthropic's Claude.

## License

Reporting and design by Dimuthu Attanayake. Data is public domain (USDA ERS).
