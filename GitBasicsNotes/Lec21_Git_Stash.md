Suppose you are in some branch (say branch1) and you are experimenting with something and it is not complete. Therefore you don't want to commit it. At the same time, suppose you have to switch to some other branch (say main) and do some work in that branch.

Because you have not staged nor committed the changes/work in branch1 your work will be lost. You don't want this to happen. In this case you can use git stash.

Use `git stash` when you want to record the current state of the working directory and the index, but want to go back to a clean working directory. The command saves your local modifications away and reverts the working directory to match the `HEAD` commit.

Commands related to this:

1. git stash
2. git stash list : All the modifications stashed away by the above command can be listed with this command.
3. git stash show : inspect all the modification stashed away by git stash command.
4. git stash apply --index : restore the modification (potentially on top of a different commit) with this command.