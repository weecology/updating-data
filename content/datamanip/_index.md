+++
title = "Add Data Code"
date = 2018-12-08T18:38:38-05:00
weight = 5
pre = "<b>5. </b>"
+++

1. Add any packages that your data cleaning and manipulation requires to
   *p_load* function call in *install-packages.R*. Do not remove any of the
   packages that are already there.
   
    ```
    # Install packages required for analysis
    # Add any packages required for you data cleaning and manipulation to the
    # `p_load` function call below
    # Do not remove the packages already listed here
    # they are important for running the livedat repository
    
    pacman::p_load(git2r, httr, semver, yaml, dplyr)
    ```
2. Modify *datascript.R* to the code you need for data cleaning and manipulation
3. Commit and push these changes to your repository
