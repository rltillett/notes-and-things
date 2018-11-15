# Committing changes to your github repository using git

The following commands assume you are operating from the project root directory.

1. Pull the newest changes from the repository before attempting to push.

    `git pull origin`

2. Stage your commit.

    `git add .`

3. Check the staged commit contains all the expected changes.

    `git status`

4. Commit the changes. A text editor will start.  Input a description of your changes and save the file.

    `git commit <-m "commit description">`

5. Push your changes to GitHub.

    `git push origin`
