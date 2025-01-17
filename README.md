<!-- README.md is generated from README.Rmd. Please edit that file -->

# plater

[![R-CMD-check](https://github.com/ropenscilabs/plater/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/ropensci/plater/actions)
[![CRAN
version](https://www.r-pkg.org/badges/version/plater)](https://cran.r-project.org/package=plater)
[![CRAN
downloads](https://cranlogs.r-pkg.org/badges/grand-total/plater)](https://cran.rstudio.com/web/packages/plater/index.html)
[![DOI](https://zenodo.org/badge/32951641.svg)](https://zenodo.org/badge/latestdoi/32951641)
[![](https://badges.ropensci.org/60_status.svg)](https://github.com/ropensci/software-review/issues/60)

plater makes it easy to work with data from experiments performed in
plates. It is aimed at scientists and analysts who deal with microtiter
plate-based instruments.

## Installation

plater is available through CRAN. Just run:

``` r
install.packages("plater") 
```

## Getting your data in

Many scientific instruments (such as plate readers and qPCR machines)
produce data in tabular form that mimics a microtiter plate: each cell
corresponds to a well as physically laid out on the plate. For
experiments like this, it’s often easiest to keep records of what was
what (control vs. treatment, concentration, sample type, etc.) in a
similar plate layout form.

But data in those dimensions aren’t ideal for analysis. That’s where
`read_plate()` and `add_plate()` come in.

- `read_plate()` takes data in plate layout form and converts it to a
  data frame, with one well per row, identified by well name.
- `add_plate()` does the same thing, but merges the new columns into an
  existing data frame you provide.

In other words, these functions seamlessly convert plate-shaped data
(easy to think about) into tidy data (easy to analyze).

To make it even easier, if you have multiple plates in an experiment,
use `read_plates()` to read them all in and combine them into a single
data frame.

## Seeing your data

Sometimes it’s useful to map your data back onto a plate (are the weird
outliers all from the same corner of the plate?). For that, there’s
`view_plate()`, which takes a data frame with one well per row, and lays
it out like it’s on a plate.

## Vignette

For a detailed example of how to use `plater`, check out [the
vignette.](https://cran.r-project.org/web/packages/plater/vignettes/plater-basics.html)

## Contributing to `plater`

`plater` is developed under a [Contributor Code of Conduct](CONDUCT.md).
To contribute to its development, you must agree to abide by its terms.
Pull requests for changes are accepted with gratitude. Please include
tests as appropriate with any pull requests.

Requests for new features and reports of bugs or security
vulnerabilities can be made
[here](https://github.com/ropensci/plater/issues) or emailed to the
address listed
[here](https://github.com/ropensci/plater/blob/master/DESCRIPTION).

[![ropensci
footer](https://ropensci.org//public_images/github_footer.png)](https://ropensci.org/)
