## pre-commit-gitleaks

pre-commit script is used for checking a local directory of your GitHub repository using gitleaks tools from https://github.com/gitleaks/gitleaks

The script can be run using curl in your local directory of the GitHub repository by performing the following command:
curl https://raw.githubusercontent.com/ivanloktionov/pre-commit-gitleaks/main/pre-commit | sh -

**Note: for Windows users, it's needed to use Git Bash tool for correct script execution.** 

## Installation of the script as pre-commit hooks

1. Download the script to your local machine into /path/to/your/git_directory/.git/hooks with the name pre-commit
2. Make the file executable: 

  ```bash
  chmod +x pre-commit
  ```
3. Enable git config hooks option in gitleaks section

  ```bash
  git config gitleaks.hooks enable
  ```
If it's needed to disable its execution during the commit perform the following

 ```bash
     git config gitleaks.hooks disable
 ```
