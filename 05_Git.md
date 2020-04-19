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
* What is a commit?
* How can history be useful?
* What does it mean to stage a file?
* What are these hashes the history?
* How can I see what has changed?
* Why do I need to keep staging files as I make changes?
* Understanding Git integrations in VS Code

## Working with branches
* What is the HEAD?
* What is a detached HEAD? (HEAD not on a named branch.)
* What is `master`? (The default branch name.)
* How do I go to another branch? (`git checkout NAME`)
* How do I create a branch?  (`git checkout -b NAME`)
* How do I know what branch I am on? (`git branch`)

## Working with remotes
* What is a remote?
* What common webservices are available?
* How do I clone an existing repository?
* What's the difference between fetch and pull?

## Pushing to upstream
* How do I push a branch?
* What is a merge?
* What is a fast-forward merge?

## Working with multiple people on one repository
* Having different branches
* Understanding `develop` and `master` + feature branches
* Can I overwrite an already pushed commit?
* Why is force pushing a bad idea?

## Recommended software

* SourceTree
* Sublime Merge
