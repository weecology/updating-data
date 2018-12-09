+++
title = "Allow Automated Updating"
date = 2018-12-08T18:38:38-05:00
weight = 4
pre = "<b>4. </b>"
+++

This set of steps creates a "Personal Access Token" that works like a password
for you GitHub account. Someone with access to this token would be able to use
it to change most of the core things in your repositories.

1. Select *Settings* from the https://github.com menu

   ![Screenshot of GitHub Settings menu](/screenshots/github_menu.png)

2. Select *Developer Settings* from the bottom of the *Personal settings* menu on
   the left of the screen

   ![Screenshot of GitHub Developer Settings menu item](/screenshots/github_personal_settings_menu.png)

3. Select *Personal access tokens* from the bottom of the menu on the left of
   the screen

   ![Screenshot of Personal access tokens menu item](/screenshots/github_pat_menu_item.png)

4. Click the *Generate new token* button in the top right of the screen

   ![Screenshot of Generate new token button](/screenshots/github_generate_new_token.png)

5. Enter a clear description of the use of this connection in the *Token description* box

   ![Screenshot of token description box](/screenshots/github_token_description.png)

6. Click the *repo* scope check box

   ![Screenshot of repo scope check box](/screenshots/github_repo_scope_checkbox.png)

7. Click the *Generate token* button at the bottom of the screen

   ![Screenshot of generate token button](/screenshots/github_generate_token.png)

8. Click the copy icon to the right of the long string of letters and numbers in
   the green box

   ![Screenshot of personal access token and copy button](/screenshots/github_pat_copy.png)

9. Go to https://travis-ci.com/ and choose your data repository from the *My Repositories* list on the left side of the screen

   ![Screenshot of My Repositories menu on Travis](/screenshots/travis_my_repos_menu.png)

10. Click the *More options* menu on the right side of the screen and select
    *Settings*

   ![Screenshot of More options menu on Travis](/screenshots/travis_more_options_menu.png)

11. In the *Environment Variables* section enter *GITHUB_TOKEN* in the *Name*
    box and paste the token you copied from GitHub into the *Value* box.

   ![Screenshot of Environmental Variables settings on Travis](/screenshots/travis_envir_vars.png)

12. Click the *Add* button at the right edge of this section

   ![Screenshot of add button on Travis](/screenshots/travis_add_button.png)
