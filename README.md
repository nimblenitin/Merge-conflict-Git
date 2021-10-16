# Merge-conflict-Git

A merge conflict is an event that occurs when Git is unable to automatically resolve differences in code between two commits.

Steps to demonstrate-

```

1. Create a sample directory and initialize it as a git repository
$ mkdir resolve-merge-conflict
$ cd resolve-merge-conflict
$ git init 

2. Creating a file with three lines in it
$ vi index.html

3. Add the file to the repository and committing it
$ git add .
$ git commit -m "Master : Added Second line"
$ git status
$ git log --oneline

4. Use the following command to create a new branch:
$ git branch feature-one
$ git checkout feature-one
$ git log --oneline

5. Use the following command to edit the index.html file and add a line:
$ vi index.html
$ git add .
$ git commit -m "Feature-one Branch: Added Third line"
$ git status

6. Switch back to the master branch
$ git checkout -

7. Use the following command to merge the file changes made in both the branches:
$ git merge feature-one

8. Open the index.html file using the following command and remomve a line added in main branch and feature-one branch:
$ vi index.html

9.  Run the following command to merge without conflict:
$ git merge feature-one

10. Using git add to stage the newly merged content and commit
$ git add .
$ git commit -m “retained the master changes while doing a merge”

```
