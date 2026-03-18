# Are Corals from Upwelling Zones Hardended Against Bleaching?
### Assessing Coral Bleaching Resistance in the Upwelling vs Non-upwelling Zone of Panama’s Pacific

### Author: Richard Montes Lemus 

## About

### Purpose:
Panama's Pacific coast offers a unique natural experiment: two adjacent regions with very different ocean conditions, separated by the Azuero Peninsula. The Gulf of Panama experiences seasonal upwelling, a process where strong winds push cold, nutrient-rich water to the surface, while the Gulf of Chiriquí remains consistently warm and stable year-round.

Scientists at the Smithsonian Tropical Research Institute have used this contrast to study how corals respond to environmental stress. This analysis focuses on two dominant coral species: Pocillopora Type 1, a slow-growing coral that tends to be more resistant to bleaching, and Type 3, a fast-growing species more vulnerable to heat stress. Together they make up roughly 90% of coral cover in Panama's Pacific.

The 2023–2024 mass bleaching event provides a real-world test of whether corals in more variable, upwelling-exposed environments are more resilient to ocean warming. This infographic compares bleaching and mortality patterns across upwelling regimes and between coral types to explore that question.

**This infographic explores the following questions:**
- Differences in coral species composition between upwelling and non-upwelling zones
- How heat stress varies over time across upwelling regimes.
- How bleaching and mortality between Pocillopora Type 1 and Type 3 vary across time in non-upwelling vs upwelling regimes.

### Highlights:
- Coral silhouette fill chart showing species composition by upwelling zone
- Dual-line degree heating weeks (DHW) graph comparing thermal stress across zones over time
- Stacked area charts tracking coral bleaching, recovery, and mortality by species and zone

### File Structure

```
├── data
│   ├── panama_pacific_east.txt
│   ├── panama_pacific_west.txt
│   └── point_data.parquet
├── drafting-viz.pdf
├── eds240-infographic.Rproj
├── exploration.pdf
├── fonts
├── infographic_assembly.html
├── infographic_blogpost.html
└── README.md

```

### Data Descriptions:

**panama_pacific_east.txt**
- NOAA Coral Reef Watch 5km virtual station time series data for Panama's Pacific East (upwelling) region, including degree heating weeks and sea surface temperature from 1985–present.

**Access:**
[NOAA Coral Reef Watch](https://coralreefwatch.noaa.gov/product/vs/gauges/panama_pacific_east.php)

**panama_pacific_west.txt**
- NOAA Coral Reef Watch 5km virtual station time series data for Panama's Pacific West (non-upwelling) region, including degree heating weeks and sea surface temperature from 1985–present.

**Access:**
[NOAA Coral Reef Watch](https://coralreefwatch.noaa.gov/product/vs/gauges/panama_pacific_west.php)

**point_data.parquet**
- Photoquadrat point-count classification data from coral reef transects collected by the Connolly Lab at the Smithsonian Tropical Research Institute. Includes coral health status (alive, bleached, dead) by species type, site, and date across upwelling and non-upwelling zones.

**Access:**
Connolly Lab, Smithsonian Tropical Research Institute

### References:

[1] NOAA Coral Reef Watch. (2025). *NOAA Coral Reef Watch 5km Regional Virtual Stations Time Series Data for Panama Pacific East* [Data file]. NOAA Coral Reef Watch, College Park, Maryland, USA. Available: https://coralreefwatch.noaa.gov/product/vs/gauges/panama_pacific_east.php. [Accessed January 20, 2025].

[2] NOAA Coral Reef Watch. (2025). *NOAA Coral Reef Watch 5km Regional Virtual Stations Time Series Data for Panama Pacific West* [Data file]. NOAA Coral Reef Watch, College Park, Maryland, USA. Available: https://coralreefwatch.noaa.gov/product/vs/gauges/panama_pacific_west.php. [Accessed January 20, 2025].

[3] Connolly Lab, Smithsonian Tropical Research Institute. *Coral reef photoquadrat point-count data, Panama Pacific* [Data file].

## Outputs

**File:**

- `drafting-viz.pdf`
  Document containing the infographic brainstorm process
- `exploration.pdf`
  Document with exploratory visualizations
- `fonts`
  Alternative fonts used for some visualizations
- `infographic_assembly.html`
  Final infographic plots
- `infographic_blogpost.html`
  Infographic blog post rough draft

**Required Tools:**
- R: `tidyverse`, `here`, `janitor`, `showtext`, `glue`, `ggtext`, `arrow`, `dplyr`, `lubridate`

Acknowledgement: 
The code and content for this analysis comes from the EDS 240 course in the Bren School of Environmental Science and Managment Master of Environmental Data Science Program. This course is led by Sam Shanny-Csik and co-led by Annie Adams.
