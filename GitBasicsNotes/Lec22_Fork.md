
Suppose you want to make some changes in some open source project (i.e, some github repo say Proj1). You can clone that project into your local git repo and make the changes locally. But then if you are not an authorized collaborator, you cannot push the local changes back to the Proj1 github repo.

In such cases you can fork Proj1 in your Github (rename it as Proj1Nir), clone it, make local changes, and push it back to Proj1Nir. This is fine since you own Proj1Nir and you don't need any permissions.

Suppose you want the changes you have made to the forked repo (i.e Proj1Nir) to be accepted globally, you can send a pull request to Proj1.

Now some collaborator from Proj1 can review your pull request and decide to either merge(accept the pull request) or not merge(reject the pull request)