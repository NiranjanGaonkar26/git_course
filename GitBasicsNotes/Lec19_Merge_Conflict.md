Conflicts generally arise when two people have changed the same lines in a file, or if one developer deleted a file while another developer was modifying it. In these cases, Git cannot automatically determine what is correct. 

Conflicts only affect the developer conducting the merge, the rest of the team is unaware of the conflict. 

Git will mark the file as being conflicted and halt the merging process. It is then the developers' responsibility to resolve the conflict.

==2 scenarios when the merge can fail==

 1. Git fails to start the merge:
    A merge will fail to start when Git sees there are changes in either the working directory or staging area of the current project. Git fails to start the merge because these pending changes could be written over by the commits that are being merged in.
    When this happens, it is not because of conflicts with other developer's, but conflicts with pending local changes. The local state will need to be stabilized using `git stash`, `git checkout`, `git commit` or `git reset`.

2. Git fails during the merge
   A failure DURING a merge indicates a conflict between the current local branch and the branch being merged. This indicates a conflict with another developers code. Git will do its best to merge the files but will leave things for you to resolve manually in the conflicted files.