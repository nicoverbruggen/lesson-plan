# Part 5: Git

## Terminology
* Repository
* Staging
* Commit
* Branch
* Merge conflict
* Merge commit
* SSH protocol
* SSH key
* SSH key-based authentication
* History
* Upstream

## Prep
* Is there a SSH key in ~/.ssh?
* Generating an SSH key for the user: `ssh-keygen -t rsa -b 4096 -C "email"`

## Understanding basics
* Why is Git a thing?
    - Git is used for version control. 
    - We can use it to keep track of changes in code over time.
    - It's decentralized so everyone keeps their own code
    - It can also be used to branch off specific changes
* What is a commit?
    - A set of changes to one or more files
    - It only contains information about what changed between now and the last commit
* How can history be useful?
    - We can go back in time to look at (now) deleted code
    - We can see what exactly has changed
* What does it mean to stage a file?
    - It means you're saying that the file, as it is right now, is ready to be committed
    - You're confirming that the changes in the file are OK to be saved
* What are these hashes the history?
    - Each historic commit has a hash that is used as a unique identifier
* How can I see what has changed?
    - Using `git diff` you can find out what's changed between now and the last commit
    - Other programs exist for looking at commit diffs
* Why do I need to keep staging files as I make changes?
    - Because every time you make a change, you're staging those specific changes
    - Subsequent (unstaged) changes need to be staged every time
* Understanding Git integrations in VS Code
    - There are good plugins available for VS Code

## Working with branches
* What is the HEAD?
    - It's where we currently are in the Git repository. The basis for your current folder and all of its contents.
    - Changes might be either staged or unstaged, see `git diff` to see what has changed
* What is a detached HEAD? 
    - HEAD not on a named branch.
* What is `master`? 
    - The default branch name.
* How do I go to another branch? 
    - `git checkout NAME`
* How do I create a branch and check it out?
    - `git checkout -b NAME`
* How do I know what branch I am on?
    - `git branch`

## Working with remotes
* What is a remote?
    - It's a server that isn't the current computer
    - It's a server that support git (usually via SSH or HTTPS)
* What common webservices are available?
    - GitHub
    - GitLab
* How do I clone an existing repository?
    - `git clone <url>` 
* What's the difference between fetch and pull?
    - Fetch only gets the remote data from the repo but doesn't integrate the changes into your local copy of the repository
    - Pull does integrate the changes

## Pushing to upstream
* How do I push a branch?
    - `git push <remote-name> <branch>` 
* How do I push a branch AND tell git about this being the upstream branch?
    - `git push -u <remote-name> <branch>` 
* What is a merge?
    - It's when there are conflicts in the history of the repository, or in specific files
* What is a fast-forward merge?
    - A fast-forward merge is a merge that merges two branches where one branch was just behind and had not previously diverged

## Working with multiple people on one repository
* Why do you need multiple branches when working on a repository?
    - To keep stable from unstable code
    - To keep features separated
    - To avoid merge conflicts
* Understanding `develop` and `master` + feature branches
    - `master` is the stable branch
    - `develop` is for unstable code
* Can I overwrite an already pushed commit?
    - Yes, by force pushing. That commit is gone then.
* Why is force pushing a bad idea?
    - Because it means that others working on the same repository will have a different history; avoid it at all costs!

## Recommended software
* SourceTree
* Sublime Merge
