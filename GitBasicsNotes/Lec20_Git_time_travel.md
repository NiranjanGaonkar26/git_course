Suppose you want to work with some older commit version (say that was the most stable version, or you want to create a lite version of the app with fewer features). You can always do this as follows:

Step 1: git checkout commit_id
This basically creates a new branch (temporary) with the files from the commit specified by the commit id.

Step 2: git switch -c branch_name
Formally creating a new branch for that temporary branch.
