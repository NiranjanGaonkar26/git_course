Suppose you have successfully implemented new features which are sitting in a different branch, therefore you want to merge the 2 branches.

follow the below steps to perform the merging of 2 branches

1. git pull origin branch_name: Firstly pull the changes on the branch from remote repo to your local git repo. This is because there will be a lot of collaborators in a large project, therefore you must first have the updated code in your local repo before you can merge the branches and push it back to the remote repo.

2. Secondly, before merging the 2 branches you have to be in the main branch first. This you can do either by git switch main or git checkout main.

3. git merge branch_name : this command will merge the specified branch with main branch.

4. Lastly push the merge to the remote repo using git push -u origin main