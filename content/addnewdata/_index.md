---
date: 2016-04-09T16:50:16+02:00
title: Add new data (manually)
weight: 9
pre: "<b>1. </b>"
---

1. Create a new branch off of the master branch for your repository.

2.  Enter new data into a file in the `new-data` folder.

    The `new-data/rodent_abundance_new.csv` file included in this template includes data with an error! Appending the new data to the old data without running checks will introduce an error to the main data file and cause the tests to fail.

3. Run `datascript.R` to perform quality checks and correct the new data.

    Running `datascript.R` in this example will flag an error in the periods:

    ```
    [1] "Unlikely period #:"
  period BA DM DO DS NA. OL OT PB PE PF PH PI PL PM PP RF RM RO SF SH SO
1   4620  0 44 24  0   5  1 11  5 10  1  1  0  1  0 92  0  1  1  0  0  0
    ```

    Uncomment and run the following line in `datascript.R` to fix the error:

    ```
    # Fix the error in the periods

    new_data[ which(new_data$period == 4620), 'period'] <- 462
    ```

    and proceed with `datascript.R` to append the new data to the main data file.

4. Commit and push these changes to your branch.

5. Open a pull request to merge your branch into the master. This will trigger Travis to run the tests you added earlier.

6. If all the checks pass, merge your pull request into the master and delete the working branch.
