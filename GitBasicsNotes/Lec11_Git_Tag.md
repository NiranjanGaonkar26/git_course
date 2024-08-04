**Git commands wrt this lecture**

1. git remote -v : gives the remote repo(s) to which our local repo is connected to.

**Git Tags**

Git has the ability to tag specific points in a repository’s history as being important. Typically, people use this functionality to mark release points (`v1.0`, `v2.0` and so on).

1. git tag : Lists the existing tags in your git repo. 

==Creating tags==

Git supports two types of tags: _lightweight_ and _annotated_.

A lightweight tag is very much like a branch that doesn’t change — it’s just a pointer to a specific commit.
Annotated tags, however, are stored as full objects in the Git database. They’re checksummed; contain the tagger name, email, and date; have a tagging message. It’s generally recommended that you create annotated tags so you can have all this information; but if you want a temporary tag or for some reason don’t want to keep the other information, lightweight tags are available too.

1. git tag -a version_number -m "message" : Create an annotated tag with the version number specified and the custom message.

2. git tag version_number: Create a lightweight tag with the version number specified.

==Sharing Tags==

By default, the `git push` command doesn’t transfer tags to remote servers. You will have to explicitly push tags to a shared server after you have created them.

1. git push origin tagname : push the tag specified by tagname to the remote repo.
   ==Note:== the tagname (i.e version name) will be of the most the recent commit (i.e, Head)
