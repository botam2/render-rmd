Untitled
================

## R Markdown

``` r
library(sf)
```

    ## Linking to GEOS 3.8.0, GDAL 3.0.4, PROJ 6.3.1

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.1 ──

    ## ✓ ggplot2 3.3.5     ✓ purrr   0.3.4
    ## ✓ tibble  3.1.2     ✓ dplyr   1.0.7
    ## ✓ tidyr   1.1.3     ✓ stringr 1.4.0
    ## ✓ readr   1.4.0     ✓ forcats 0.5.1

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
data <- st_read('../gpkg/lomas_serfor.gpkg')
```

    ## Reading layer `lomas_serfor' from data source 
    ##   `/home/barja/Documentos/Portafolio/rgee_dashboard/yup/yup/gpkg/lomas_serfor.gpkg' 
    ##   using driver `GPKG'
    ## Simple feature collection with 19 features and 9 fields
    ## Geometry type: MULTIPOLYGON
    ## Dimension:     XY
    ## Bounding box:  xmin: -77.10384 ymin: -12.38606 xmax: -76.6727 ymax: -11.78022
    ## Geodetic CRS:  WGS 84

``` r
plot(st_geometry(data))
```

![](fig/unnamed-chunk-1-1.png)<!-- -->
