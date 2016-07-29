#Git - Merging and Teams
Few of those problem that every beginner faces in his software development career, how does git branching and merging works. But before knowing branching there is a thing that confused me, like what happens when two people starts working on same branch and a member try pushing repository and he get an error message like,

` remote repository contains changes which do not exist locally `

In above case git will either ask you to pull the repository first or stash the changes. So what happened exactly, actually any other team member pulled that repository before you and made some changes to repository and pushed, creating a bit of a history that your locally repository do not have.

So what are the things that should be kept in mind while working in team, there are two (in my opinion):
* First pull every time before starting to work on repository, this will keep you on the latest branch position
* But what if you forget to push your changes last time and this time while pulling you faced the error like above, explained below

##Merge Commit
This is happening because now your git graph have two histories or branches, one locally with you and other remotly on github. So, now you have to merge them so that succeeding graph can have a history about both of these branches with there respective edits. Best thing to do, pull the remote branch, now this will do two things,
* One, this will fetch all the changes existing remotely and,
* Other this will merge that branch to your existing one locally creating a single branch further on.

Now you can push your repository. But this time git have to show the difference between present and preceding commit from either of the parents so you can see two identical commits depending on which commit git chose.
