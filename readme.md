##  What is Version Control?
Version control is a system that records changes to a file or set of files over time so that 
you can recall specific versions later.

## What is git? How does it work?
Git is a DevOps tool used for source code management. It is a version control system that is used to track changes in the source code, enabling multiple developers to work together on non-linear development.


## What does `'git init'` do?
The `'git init'` command creates a new repository.

## What does `'git status'` do?
The `'git status'` command displays the state of the working directory and the staging area.

## What does `'git add'` do?
The `'git add'` command adds a change in the working directory of the staging area.

## What does `'git commit'` do?
The `'git commit'` command captures a snapshot of the project's currently staged changes.

## What does `'git log'` do?
The `'git log'` command displays committed snapshots.

## What does `'git diff'` do?
The `'git diff'` command helps you see, compare and understand changes in your project.

## What is `'.gitignore'` and why should we use it?
The `'.gitignore'` command ensures that certain files not tracked by Git remain untracked.We should use it as it allows us to custom-tailor our folders based on the types of files that need to be included.

## Distributed Version Control

![](E:\Documents-SG\Github\git_learning\Images\CVC_vs_DVC_Diagram.PNG)
This diagram showcases the working style of both CVC and DVC. CVC work from one online repo, where users commit and update from thier own working copies. DVC operates with both a local repo and an online repo. This allows users to commit and update copies to their own local repo's, before pushing this onto the online repo.

## What is Github?
Github is a collaborative version control system. This allows multiple people to make separate changes to code at the same time, as the changes are stored on the local repositories as opposed to the online one.

## What are alternative options?
An alternative to Github is Bitbucket. Bitbucket is a Git-based code and a CI/CD tool optimised for teams that use Jira. Bitbucket arguably has more built-in flexibility than Github, hence why some development teams opt for it instead.
## How do you link a local repo to a remote repo on Github?
Copy the following steps in order to link a local repo to a remote repo on Github:
* Create a new repository on the Github website.
* Enter the following on Gitbash:
* `git remote add origin git@github.com:Username/RepositoryName`
* `git branch -M main`
* `git push -u origin main`

## How do you link a remote repo to a new local repo?
Copy the following steps in order to link a remote repo to a new local repo:
* Create a new local repo using the `git init` command where you want to initialise the repo.
* Add files to the repo using `git add`
* Commit the files using `git commit` 
* Link the remote repo with `git remote add <name_of_repo> <URL_of_repo>`
* Verify the remote repo with `git remote -v`
* Push your changes to the repo using `git push <remote_name> <branch_name>`