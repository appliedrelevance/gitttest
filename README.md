# This is a test of how to do git.

This will be put up into a Coda document to document how our devops work.

1. Step one is init the git repository.

    ```
    cd gittest
    git init
    ```

1. Next, make the initial commit.

    ```
    git commit -a -m "Make more changes to README".
    ```

1. Add repository to github

    ```
    echo "# gitttest" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin https://github.com/appliedrelevance/gitttest.git
    git push -u origin main
    ```

1. Finally, commit and push all these changees to the origin repository main branch.

    ```
    git commit -a -m "final commit to initialize the document"
    git push -u origin main
    ```

That should have created a repository in the github cloud that is synchronized with the local clone of the repository. 

## Make a change to the existing code.

Making a change to the existing code starts with deciding which ticket to work on.  Each ticket has a number in the project sprint board, whether it is in Jira or Coda.  Since we are currently using Coda.io, that's what we will use for this example.  

1. If necessary, configure git to merge pulls by default.

    ```
    git config --global pull.rebase false
    ```

1. Pull the master/main changes down to the local version if necessary. 

    ```
    git pull
    ```

1. I've made changes and committed in the cloud.  What happens now if I try to commit these changes?


