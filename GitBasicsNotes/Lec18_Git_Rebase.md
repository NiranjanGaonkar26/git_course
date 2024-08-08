git merge and git rebase both are methods to merge a branch with main.

Suppose you have 2 branches main and branch1. You do some commits on main and some commits on branch1 independently. => the commit log checkpoints will be branched (i.e, it will not be a straight tree, rather a branched tree).

Now when you merge the 2 branches, of course all the changes/ updates from branch1 will be incorporated in main, however commit history log will not be a clean tree. In some cases you might not want this to happen. In that case use git rebase.

1. git pull origin branch_name: Firstly pull the changes on the branch from remote repo to your local git repo. This is because there will be a lot of collaborators in a large project, therefore you must first have the updated code in your local repo before you can merge the branches and push it back to the remote repo.

2. Secondly, before merging the 2 branches you have to be in the main branch first. This you can do either by git switch main or git checkout main.

3. git rebase branch_name : this command will merge the specified branch with main branch.

4. Lastly push the merge to the remote repo using git push -u origin main
