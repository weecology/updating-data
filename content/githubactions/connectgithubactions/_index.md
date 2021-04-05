+++
title = "Connect to GitHub Actions"
date = 2018-12-08T18:38:38-05:00
weight = 4
pre = "<b>4. </b>"
+++

1. Go to your version of the repo on GitHub and click the Actions tab
  ![Screenshot of GitHub Actions tab](/screenshots/github_actions_tab.png)
1. Under "All workflows" you should see your commit message with either:
    + A yellow spinning ball indicating a particular workflow is currently running. Your first commit should take a little over 6 minutes to complete.
    + A green checkmark indicating the workflow was successful.
    + A red X indicating the workflow failed
  ![Screenshot of Workflow Run](/screenshots/github_actions_workflow_run.png)
1. To get details of a particular workflow, click on the commit message -> R CMD CHECK
  ![Screenshot of Workflow Run](/screenshots/github_actions_R_CMD_CHECK.png)
