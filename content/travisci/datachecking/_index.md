---
date: 2016-04-09T16:50:16+02:00
title: Add data checks
weight: 8
pre: "<b>8. </b>"
---

1. Modify the .R scripts in the `testthat` folder to automatically check your data for errors. For example, copy [this script](/sample-scripts/test-periods.R) into `testthat/test-periods.R`. It will automatically make sure that the sampling period values in your data are plausible.

  ```
  library(testthat)
  library(dplyr)
  context("checks that period values are valid")

  base_data <- read.csv('../data/rodent_abundance.csv',
                        stringsAsFactors = F)

  test_that("period numbers are valid", {

    expect_true(all(base_data$period < 1000))

  })
  ```

2. Add, commit, push, and double-check that your changes are now on GitHub:
  ![Screenshot of test on GitHub](/screenshots/github_add_test.png)
3. Travis will automatically run your tests. If there are errors, the build will fail. Check to see that your tests have passed:
  ![Screenshot of Travis passing](/screenshots/travis-add-test-passed.png)
