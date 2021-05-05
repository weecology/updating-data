+++
title = "Add Data Code"
date = 2018-12-08T18:38:38-05:00
weight = 7
pre = "<b>7. </b>"
+++

1. Add any packages that your data cleaning and manipulation requires to the `DESCRIPTION` file in your package's root. For example, we've just added the `dplyr` and `tidyr`. Note: Unfortunately you cannot add the `tidyverse` umbrella package as this will cause the package check to fail: you need to install the packages you want to use individually.
  ![Screenshot of DESCRIPTION file](/screenshots/github_actions_R_CMD_CHECK.png)
2. Modify *datascript.R* to the code you need for data cleaning and manipulation
2. In `.github/workflows/R-CMD-check.yaml` add the following code at the end of the file
```
      - name: Run datascript
        run: Rscript datascript.R
```
3. Commit and push these changes to your repository
