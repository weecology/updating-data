---
date: 2016-04-09T16:50:16+02:00
title: Create tests
weight: 8
pre: "<b>1. </b>"
---

1. Modify the .R scripts in the `testthat` folder to check that the data in your main `data` folder meets your quality checks.

    For example, this template includes scripts to confirm that the data meets the same quality checks as above - namely, the column names are as expected (`testthat/test-colnames.R`), and the sampling period values are plausible (`testthat/test-periods.R`.)

2. Commit and push these changes to your repository
