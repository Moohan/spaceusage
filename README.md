
# spaceusage

<!-- badges: start -->
<!-- badges: end -->

Space usage was intended to get and plot drive usage. As a side affect it can
also get the full names of users with a given group membership.

See [the documentation](https://moohan.github.io/space_usage/).

## Installation

You can install this package from GitHub with using {`remotes`} or {`pak`}

``` r
install.packages("pak")
pak::pak("Moohan/spaceusage")
```

## Analysing space usage

Get usage data for a given drive.

``` r
library(spaceusage)

hscdiip_usage <- get_usage("hsdiip")
```

Plot the usage.

```r
plot_usage(hscdiip_usage)
```

## Checking on users in certain groups

Who has access to a certain group.

```r
get_group_membership("hscdiip")
```
