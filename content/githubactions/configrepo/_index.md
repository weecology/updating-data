+++
title = "Configure the Repository"
date = 2018-12-08T18:38:38-05:00
weight = 2
pre = "<b>2. </b>"
+++

1. Open the repo in RStudio by clicking the *.Rproj* file that has the name of your new repository.
1. If you haven't already, install the *usethis* R package.
1. Run `usethis::use_github_actions()`. This should create a directory called *.github/* as well as a *.Rbuildignore* file. 
1. Open the *DESCRIPTION* file. Under *Authors@R* replace Cosme Fulantino's name with yours. Feel free to add an email as well as an ORCID if you like.
1. In the root directory of the repository open the *config.yml* file
2. Change the repo name to that for your project. This should be the GitHub user
   or organization name followed by the repository name. You can get this by
   removing the "https://github.com/" from the url for your repository.
3. Change the deploy email and username. These values will identify the user
   that is shown as making the automated commits. Generally you want these to be
   different from your user account so it is clear which commits are
   automated. You don't need a GitHub account for this user, this is just the
   name and email that will appear in the commit log.
4. Commit and push these changes to your GitHub repository.

<!--
TODO: Fix deploy email and username
-->
