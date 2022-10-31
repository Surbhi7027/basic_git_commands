### Basic Git commands
Creating a repository

    Creating a new local repository from scratch
    $ git init [project name]

    Downloading from an existing repository
    $ git clone my_url

Observing your repository

    Listing new or modified files that are not being committed yet.
    $ git status

    Displaying the file changes that are not being staged
    $ git diff

    Display the change to the staged files
    $ git diff --cached

    Display all the staged and unstaged file changes
    $ git diff HEAD

    Display the differences between two commit ids
    $ git diff commit1 commit2

    Listing the dates and the author of the changed file
    $ git blame [file]

    Display the file changes for a particular id or a file
    $ git show [commit]:[file]

    Display the complete change history
    $ git log

    It will display the change history for a particular file or a directory
    $ git log -p [file/directory]

Working with branches

    It will display all the local branches
    $ git branch

    It will display all the local as well as the remote branches
    $ git branch -av

    It will switch to a branch and will update the working directory accordingly
    $ git checkout my_branch

    It will create a new branch named new_branch
    $ git branch new_branch

    It will delete the branch named my_branch
    $ git branch -d my_branch

    It will merge two branches, branch_a, and branch_b
    $ git checkout branch_b
    $ git merge branch_a

    It will tag the current commit.
    $ git tag my_tag

Making changes

    To stage the file and ready to commit
    $ git add [file]

    It will stage all the changed file and ready to commit
    $ git add .

    It will commit all the staged files to the versioned history
    $ git commit -m “commit message”

    It will commit all the tracked file to the versioned history
    $ git commit -am “commit message”

    It will unstage the file and keep the file changes
    $ git reset [file]

    It will revert everything to the last commit
    $ git reset --hard

Synchronize

    It will get the latest changes from the origin
    $ git fetch

    It will fetch the latest changes from the origin and merge
    $ git pull

    It will fetch the latest changes from the origin and rebase
    $ git pull --rebase

    It will push the local changes to the origin
    $ git push

Help command

    Use the git help command for more details $ git command --help
