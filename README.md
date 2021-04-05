# Updating Data Website

[![Netlify Status](https://api.netlify.com/api/v1/badges/45a77fe8-6fdf-4908-9f8e-934085bdc488/deploy-status)](https://app.netlify.com/sites/updating-data/deploys)

Hugo website for instructions on how to make a regularly updating data pipeline using R, git, GitHub, Zenodo, and either GitHub Actions or Netlify.

In order to deploy this site locally:

1. Install [Hugo](https://gohugo.io/getting-started/quick-start/)
1. Open `config.toml` and edit the change `theme = "learn"` to `theme = "hugo-theme-learn"`
1. Unzip the contents of `themes/hugo-learn-theme.zip` so that a directory `themes/hugo-learn-theme/` gets created
1. From the Terminal, run `hugo server` from the root directory of your repo
1. Copy the `localhost` url into your browser. Ex: `localhost:1313/`
