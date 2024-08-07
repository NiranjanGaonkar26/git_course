Say you have some working code in the main branch. Suppose you want to experiment with a new feature, but the working code may fail when you push the changes (of course you can switch between the branches). 

So it is better to create a new branch (which will have all the directories/files from the main branch) and try out you experimental code there.

1. Creating a new branch

	i. git checkout -b new_branch_name            (old version)
				or
	ii. git switch --create new_branch_name     (new version, short form is git switch --c new_branch_name)

	Both these commands create a branch and switch to that branch.

2. git checkout branch_name : switch to the specified branch

3. git branch : verifying the present branch you are in

4. git push origin new_branch_name: push your changes/ updates to the specified branch in the remote repo.


