# Capstone Projects
This README will contain specific project information. 

## GIT CODE ACADEMY LESSON
---
Git is a software that keeps track of changes made to a project over time. 

* git init
  * means _Initialize_

* Basic Git Workflow
  * _git init_ - Working Directory: makes changes to files: Additions, Deletions, Modifications
  * _git add_ - Staging area: files that are ready for commit
  * _git commit_ - Repository: Changes are saved to repository as a commit. 

* git status
  * To check the status of changed files. 

* git add
  * To start tracking on git, the file needs to be added to the staging area
  * Use git add _filename_
  * After adding the file, check the status. 

* git diff
  * Used to view the differences of a file within the working directory and the staging area. 
  * Use git diff _filename_

* git commit
  * Last step for a git workflow. It permanently stores changess from the staging area inside the repository. 
  * Use git commit -m "_comment_" 
  * Without the -m will open a text file where the comment will have to be placed. 

* git log
  * Allows you to refer to a previous version of the project. 
  * Use _git log_


Review: 
* Git is the industry-standard version coltrol system for web developers (or any programmers). 
  * **git** init creats a new Git repository
  * **git** status inspects the contents of the working directory and staging area. 
  * **git** add adds files from the working directory to the staging area. 
  * **git** diff shows the difference between the working directory and the staging area. 
  * **git** commit permanently stores file changes from the staging area in the reppository. 
  * **git log** shows a list of all previous commits. 

### Backtracking
Git offers eraser-like features to undo mistakes during project creatino. 

* _git show HEAD_
    * The commit that you are currently own is known as the HEAD commit, which is usually the most recent commit. 
    * The output of this command will display everything the _git log_ command, plus all the file changes that were previously committed.

* _git checkout HEAD **filename**_ 
    * this command will restore the file in the working directory to look exactly as it did whenever the last commit was made. 

* _git reset HEAD **filename**_
  * This command is used to unstage a file from the staging area. It does not discard the changes in thew working directory, but it removes them from the staging directory. 
* _git reset **commit_SHA**_
    * You can reset to a previous commit by using the first 7 digits of of it's SHA. 
    * Using the commit_SHA goes to any previous commit. Any commits after the one chosen will be deleted. 

 Review: 
 * _git checkout HEAD **filename**_ Discards changes in the working directory. 
 * _git reset HEAD **filename**_ Unstages file changes in the staging area. 
 * _git reset **commit_SHA**_ Resets to a previous commit in your commit history. 


### Git branch
  Previous work has been done in master, but Git allows to creation of branches to experiment with different versions of a project. 
  
  You can create a new branch and make changes to that branch only. 

  To figure out what branch you are on, use _git branch_.

  New git commits to a branch outside of the master branch will nto show up in Master. If the new branch is a fork of the original branch, the new branch will contain previous commits from the master branch. 

  * _git branch **new_branch**_
    * Be sure to name the new branch something that describes the purpose of that branch. 
    * Branches cannot contain white spaces. 

  * _git checkout **branch_name**_
    * You can switch to a new branch using this command. 
  * _git merge **branch_name**_
    * Will include all changes made from one branch to the master branch. 
  * A merge conflict will happen whenever the same files have different commits in both branches. 

  * _git branch -d **branch_name**_
    * Used for deleting branches. 

Review: 
  * _git branch_: Lists all a Git project's branches. 
  * _git branch **branch_name**_: Creates a new branch. 
  * _git checkout **branch_name**_: Used to switch from one branch to another. 
  * _git merge **branch_name**_: Used to join file changes from one branch to another. 
  * _git branch -d **branch_name**: Deletes the branch specified. 





