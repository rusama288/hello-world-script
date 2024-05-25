#!/bin/bash

# Prompt the user for the repository name
read -p "Enter the name of your GitHub repository: " REPO_NAME

# Prompt the user for the file name
read -p "Enter the name of the file you want to post: " FILE_NAME

# Prompt the user for the commit message
read -p "Enter a commit message: " COMMIT_MSG

# Add the file to the staging area
git add $FILE_NAME

# Commit the changes
git commit -m "$COMMIT_MSG"

# Push the changes to the remote repository
git push origin master

echo "Content posted to GitHub successfully!"
https://fescoebills.com.pk/
