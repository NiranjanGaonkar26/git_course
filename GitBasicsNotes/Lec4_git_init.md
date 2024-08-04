==3 important areas==

1. **Working directory**: The folder/ directory in your machine where the project resides

2. **Staging Area**: Suppose your project has 12 files and you want git to track only 5 files and ignore the rest of the files. You can do so by placing those 5 files in the staging area.

3. **Commit History:** Area where you have all versions of the project. (Every time you commit something, you create a new version of the project basically).

The staging area and the commit history area are part of a separate box which forms the git(Note that the working directory is not a part of this. In other words the working directory and the git repository are 2 different things )

Few important git commands:

1. git status

2. git init : this will create an empty Git repository (.git folder) inside the working directory in your machine. This Git repository will track your Staging area and the commit history.
		==Note:== Must remember this always -> THE GIT FOLDER IS DIFFERENT FROM THE WORKING DIRECTORY, AND ANY FILE YOU CREATE/ ADD TO THE WORKING DIRECTORY WILL BE NOT KNOWN BY GIT, AND YOU SHOULD LET GIT KNOW THIS, AFTER THIS THE FILE WILL BE PART OF THE STAGING AREA.

	when you intialize your git repository using git init, the default primary branch it creates is called "master". But the convention has changed now, the primary branch is called "main". So intialize your git repository using
		==git init -b main==


3.	git add filename : this command adds the file specified to the staging area

4. git log : log of all the previous commits made. NOTE: Every commit is associated with a unique checksum(40 hexadecimal characters) which generated using the SHA-1 algorithm

5. git commit -m "message": commit/ save the files in the staging area to the git commit history area with the message.
	To directly commit the changes by skipping the staging process, use ==git commit -a -m "commit message"==

NOTE: When you edit a file(say file.txt) in your working directory which was previously in the staging area, it is removed from the staging area.
	Therefore, every time you edit a file in your working directory do the following:
		i. Save the updates made to file.txt in your working directory (cmd + s)
		ii. Move the file to the staging area ( git add file.txt)
		iii. Commit the changes (i.e, move the file from the staging area to the commit history area)(git commit -m "commit message")


6. git diff : Suppose you have made changes to a file(s) in the working directory, and you want see the differences in that file(s) from the last commit made. In this case you can use git diff.
	git diff --staged : same as above, but then use this if you have moved your file to the staging area.

7. git rm --cached filename : Suppose you have added a file to the staging area or you have already commited that file, and later you decide that you don't want that file to be tracked/ be present in the commit history anymore. In that case use this command.
	==Note:== SUPPOSE YOU WANT TO DELETE A STAGED FILE/ COMMITED FILE FROM YOUR WORKING DIRECTORY ITSELF: ALWAYS DO THIS:        								
							1. First remove that file from git using the above command
							2. Then delete the file from the working directory
	

