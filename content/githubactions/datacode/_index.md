+++
title = "Add Data Code"
date = 2018-12-08T18:38:38-05:00
weight = 7
pre = "<b>7. </b>"
+++

1. Add any packages that your data cleaning and manipulation requires to the `DESCRIPTION` file in your package's root. Note: Installing R packages can be slow and so you should only install the specific packages you need, not umbrella packages like `tidyverse` (in fact installing `tidyverse` will cause the system to timeout and therefore fail). For example, we've just added the `dplyr` and `readr` packages:  
![Screenshot of DESCRIPTION file](/screenshots/github_actions-DESCRIPTION.png)
2. Modify `datascript.R` to the code you need for data cleaning and manipulation
2. Open the `.github/workflows/R-CMD-check.yaml` file. If you are using RStudio you may need to enable "Show Hidden Files" to locate this file:  
![Screenshot of show hidden files](/screenshots/github_actions-show-hidden-files.png)
2. Add the following code at the end of the file  
    ```
          - name: Run datascript
            run: Rscript datascript.R
    ```  
    so that in the end your file looks like this (in particular the spacing at the beginning of each line):  
![Screenshot of R-CMD-check.yaml](/screenshots/github_actions-yaml.png)
3. Commit and push these changes to your repository
