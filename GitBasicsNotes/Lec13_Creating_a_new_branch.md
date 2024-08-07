Say you have some working code in the main branch. Suppose you want to experiment with a new feature, but the working code may fail when you push the changes (of course you can switch between the branches). 

So it is better to create a new branch (which will have all the directories/files from the main branch) and try out you experimental code there.

1. Creating a new branch

	i. git checkout -b new_branch_name            (old version)
				or
	ii. git switch --create new_branch_name     (new version, short form is git switch -c new_branch_name)

	Both these commands create a branch and switch to that branch.

2. git checkout branch_name or git switch branch_name: switch to the specified branch

3. git branch : gives a list of all the branches in the local repo as well as the info regarding the current branch you are in.
   git branch -all : same as above, but it also lists all the branches in the remote repo as well.

5. git push origin new_branch_name: push your changes/ updates to the specified branch in the remote repo.

6. git branch -d branch_name (or git branch --delete branch_name) : deletes the specified branch from the local repo.

7. git push -u origin branch_name : If the specified branch does not exist in the remote repo, this command will create a new branch in that remote repo and pushes the changes/updates in the commit history area to that newly created branch.
   If the specified branch is already there, then it simply pushes the changes/updates in the commit history area to that newly created branch. 


