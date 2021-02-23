---
date: 2016-04-09T16:50:16+02:00
title: Add data
weight: 6
pre: "<b>6. </b>"
---

1. Add the initial version of your data to `data.csv` file in a `data` folder. For example, you can copy [this data](/sample-data/starting-data.csv) into `data/data.csv` in your copy of the template:

| period | BA | DM | DO | DS | NA. | OL | OT | PB | PE | PF | PH | PI | PL | PM | PP | RF | RM | RO | SF | SH | SO |
|--------|----|----|----|----|-----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|
| 27     | 0  | 16 | 0  | 11 | 1   | 6  | 12 | 0  | 2  | 2  | 0  | 0  | 0  | 0  | 3  | 0  | 0  | 0  | 0  | 0  | 0  |
| 28     | 0  | 15 | 5  | 15 | 5   | 4  | 10 | 0  | 3  | 1  | 0  | 0  | 0  | 0  | 2  | 0  | 1  | 0  | 0  | 0  | 0  |
| 29     | 0  | 25 | 3  | 11 | 4   | 9  | 10 | 0  | 5  | 5  | 0  | 0  | 0  | 1  | 1  | 0  | 5  | 0  | 0  | 0  | 0  |
| 30     | 0  | 35 | 7  | 11 | 5   | 15 | 9  | 0  | 1  | 8  | 0  | 0  | 0  | 0  | 0  | 0  | 6  | 0  | 0  | 0  | 0  |
| 31     | 0  | 19 | 6  | 11 | 1   | 10 | 4  | 0  | 3  | 7  | 0  | 0  | 0  | 0  | 0  | 0  | 11 | 0  | 0  | 0  | 0  |
| 32     | 0  | 23 | 1  | 23 | 1   | 6  | 5  | 0  | 2  | 10 | 0  | 0  | 0  | 0  | 0  | 0  | 10 | 0  | 0  | 0  | 0  |
| 33     | 0  | 22 | 2  | 26 | 1   | 6  | 5  | 0  | 1  | 11 | 0  | 0  | 0  | 0  | 1  | 0  | 6  | 0  | 0  | 0  | 0  |
| 34     | 0  | 23 | 3  | 36 | 9   | 5  | 1  | 0  | 1  | 6  | 0  | 0  | 0  | 0  | 2  | 0  | 0  | 0  | 0  | 0  | 0  |
| 35     | 0  | 21 | 6  | 30 | 4   | 2  | 4  | 0  | 2  | 3  | 0  | 0  | 0  | 0  | 3  | 0  | 0  | 0  | 0  | 0  | 0  |
| 36     | 0  | 15 | 6  | 16 | 4   | 1  | 2  | 0  | 2  | 4  | 0  | 0  | 0  | 0  | 1  | 0  | 0  | 0  | 0  | 0  | 0  |

  This is a subset of the Portal rodent abundance data, from sampling period 27 until sampling period 36. The two-letter column names stand for rodent species.


2. Add, commit, and push your changes to GitHub.

3. Check and see if everything is working properly:

  * Your new data are now in your repo on GitHub (go to www.github.com/YOUR_USERNAME/livedat/data)
    ![Screenshot of data.csv](/screenshots/github-add-data.png)
  * Travis is running or has completed
    ![Screenshot of Travis passing](/screenshots/travis-add-data-passed.png)

  * Your data are on Zenodo
