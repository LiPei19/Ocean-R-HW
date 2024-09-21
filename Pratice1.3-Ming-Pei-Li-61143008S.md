Practice 1.3
================
Ming Pei Li
2024-09-21

### Detailed help on the use of function

``` r
?median # alternative 1 
help (median) # alternative 2
```

### Set current working directory

``` r
knitr::opts_knit$set(root.dir = "D:\\碩士資料庫\\碩三上課程\\Ocean R\\data")
```

package::function

### Deleting all objects using rm()

``` r
rm (list = ls ())
```

### Store table in an object called “fish”

``` r
library (readxl)
fish <- read_excel("20240910\\reef_fish.xlsx") 
```

### Importing a .txt file, use read.table ()

``` r
fish <- read.table ("20240910\\reef_fish.txt", header = TRUE, sep = '\t', dec = '.') 
```

### Make a simple plot

``` r
barplot (fish$richness, main = "Top 10 reef fish Richness (Allen, 2000)", horiz = TRUE, names.arg = fish$country, cex.names = 0.5, las = 1)
```

![](Pratice1.3-Ming-Pei-Li-61143008S_files/figure-gfm/unnamed-chunk-6-1.png)<!-- -->
