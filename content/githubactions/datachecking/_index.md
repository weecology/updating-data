---
date: 2016-04-09T16:50:16+02:00
title: Add Data Checks
weight: 7
pre: "<b>7. </b>"
---


1. Modify the .R scripts in the `testthat` folder to automatically check your data for errors. GitHub Actions will automatically run any R script files inside the `testthat` folder. For example, copy [this script](/sample-scripts/test-periods-ga.R) into `testthat/test-periods-ga.R`. It will automatically make sure that the sampling period values in your data are plausible.  
    ```{r}
    library(testthat)
    library(dplyr)
    library(readr)
    context("Checks that all values in period variable are valid.")
    
    base_data <- read_csv("../data-raw/data.csv")
    
    test_that(
      desc = "Period values are valid.",
      code = {
        all_period_values_valid <- all(base_data$period < 1000)
        expect_true(all_period_values_valid)
      }
    )
    ```
2. In `.github/workflows/R-CMD-check.yaml` add the following code at the end of the file, being once again mindful of the spacing at the beginning of each line
    ```
          - name: Run tests
            run: Rscript testthat.R
    ```
2. Add, commit, push, and double-check that your changes are now on GitHub:  
![Screenshot of test on GitHub](/screenshots/github_actions-github_add_test.png)
3. GitHub actions will automatically run your tests. If there are errors, the build will fail. Check to see that your tests have passed:  
![Screenshot of GitHub Actions passing](/screenshots/github_actions-add-test-passed.png)


