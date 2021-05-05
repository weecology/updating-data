+++
title = "Keep Collecting Data!"
date = 2019-01-29T18:38:38-05:00
weight = 10
pre = "<b>10. </b>"
+++

You're done setting up your data repository! Keep adding new data, and new tests as they become necessary. Be sure to

* Add any packages you use to the `DESCRIPTION` files as we did in [Add Data]({{< ref "githubactions/adddata/_index.md" >}} "Add Data"). Recall you can't add the `tidyverse` umbrella package, you need to add its component packages individually.
* Add all testing R scripts you want to run to the `testthat` folder as we did in [Add Data Checks]({{< ref "githubactions/datachecking/_index.md" >}} "Add Data Checks").
* Add all non-testing R scripts to the main folder and add the corresponding code to `.github/workflows/R-CMD-check.yaml` as we did [Add Data Code]({{< ref "githubactions/datacode/_index.md" >}} "Add Data Code").

For more details about

* This automated workflow, see the paper: [Yenni GM, Christensen EM, Bledsoe EK, Supp SR, Diaz RM, White EP, et al. (2019) **Developing a modern data workflow for regularly updated data.** PLoS Biol 17(1): e3000125.](https://doi.org/10.1371/journal.pbio.3000125)
* Using GitHub Actions for the R language, see this [resources page](https://github.com/r-lib/actions)
* The `testthat` package, see the [package homepage](https://testthat.r-lib.org/)
