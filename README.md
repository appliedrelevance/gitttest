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



