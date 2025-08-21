## Dixie Fire Burn Severity And Vegetation Recovery Mapping
This project sought to assess post-fire damage following the 2021 Dixie Fire in Northern California. The objectives were to:
1. Map burned area and severity using spectral indices like Normalized Burn Ration (NBR).
2. Monitor vegetation recovery using spectral indices like Normalized Vegetation Difference Index (NDVI) and Enhanced Vegetation Index (EVI).
3. Monitor changes in land cover. 

## Data and Study Period
[1. Harmonized Landsat Sentinel (HLS)](https://search.earthdata.nasa.gov/search?q=hls)

[2. Dynamic World](https://dynamicworld.app/)

[3. MTBS Burned Area Boundaries](https://burnseverity.cr.usgs.gov/products/mtbs)

The study period ranged from 2020 to 2024. 

## Method
1. Median image composites were generated for all raster datasets (HLS and dynamic world).
   
2. To characterize burn severity, the difference NBR between pre- and post-fire image composites were used. Pre-fire NBR was generated from the 2020 August HLS composite, during the peak of the season. Although the fire was declared 100% contained on Oct 25th 2021 according to [CAL Fire](https://www.fire.ca.gov/incidents/2021/7/13/dixie-fire), post-fire NBR was generated from the 2021 Oct 15 to Nov 15 HLS composite to limit regrowth bias in capturing burn severity. On this [NASA page](https://svs.gsfc.nasa.gov/4993), the fire perimeter was mentioned to be contained mid-September, as could also be seen in the visualization.  This allowed the use of images from October to ensure minimal atmospheric disturbances from smoke. 
The burn severity classification scheme was adopted from the [UN-SPIDER](https://un-spider.org/advisory-support/recommended-practices/recommended-practice-burn-severity/in-detail/normalized-burn-ratio) recommended practices for evaluating burn severity.

3. Time series of seasonal(August, except for the fire year which was from Oct 15 to Nov15) median NDVI from 2020 to 2024 was plotted to assess vegetation regrowth over the affected areas.

4. Seasonal composites of Dynamic World was used to evaluate changes in land cover.

This project was carried out in GEE Python API.
