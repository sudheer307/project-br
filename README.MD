branch:
-------
Branching is a feature available in most modern version control systems. Branching in other VCS's can be an expensive operation in both time and disk space. In Git, branches are a part of your everyday development process. Git branches are effectively a pointer to a snapshot of your changes. When you want to add a new feature or fix a bug—no matter how big or how small—you spawn a new branch to encapsulate your changes. This makes it harder for unstable code to get merged into the main code base, and it gives you the chance to clean up your future's history before merging it into the main branch.


How it works:
--------------
A branch represents an independent line of development. Branches serve as an abstraction for the edit/stage/commit process. You can think of them as a way to request a brand new working directory, staging area, and project history. New commits are recorded in the history for the current branch, which results in a fork in the history of the project.

The git branch command lets you create, list, rename, and delete branches. It doesn’t let you switch between branches or put a forked history back together again. For this reason, git branch is tightly integrated with the git checkout and git merge commands.


Commands:
---------
1.git branch
      List all of the branches in your repository

2.git branch <branch>
      Create a new branch called <branch>. This does not check out the new branch  

3.git branch -d <branch>
      Delete the specified branch. This is a “safe” operation in that Git prevents you from deleting the branch if it has unmerged       changes.

4.git branch -D <branch>
      Force delete the specified branch, even if it has unmerged changes. This is the command to use if you want to permanently throw       away all of the commits associated with a particular line of development.

5.git branch -m <branch>
      Rename the current branch to <branch>.

6.git branch -a
      List all remote branches

7.git checkout <branchname>
      switched between the branches

8.git checkout -b <newbranch>
      By using this command create a new branch and switched to branch which we are created the branch at a time

9.git merge <branch>
      This command merges the specified branch into the current branch, but always generates a merge commit (even if it was a               fast-forward merge). This is useful for documenting all merges that occur in your repository.

10.git log
       To dispaly the commit messages

11.git log --oneline
       to display all the commits single page 

