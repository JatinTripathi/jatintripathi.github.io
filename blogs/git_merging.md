#Git - Merging and Teams
Few of those problem that every beginner faces in his software development career, how does git branching and merging works. But before knowing branching there is a thing that confused me, like what happens when two people starts working on same branch and a member try pushing repository and he get an error message like
` remote repository contains changes which do not exist locally `
In above case git will either ask you to pull the repository first or stash the changes. So what happened exactly, actually any other team member pulled that repository before you and made some changes to repository and pushed, creating a bit of a history that your locally repository do not have.
So what are the things that should be kept in mind while working in team, there are two:
*First pull everytime before starting to work on repository, this will keep you on the latest branch position
*But what if you forget to push your changes last time and this time while pulling you faced the error like above, explained below
