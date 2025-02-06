### Notes

Using `git cherry-pick <branch-name>`, will take the HEAD commit of the branch, and place it at the tip of your local branch.
Using `git cherry-pick <SHA-value>`, will take the commit specific to the SHA provided and place it at the tip of your local branch.


- Cherry picking a merge commit causes some complications, such as an empty commit message without the merge changes causing an empty commit.
- It's probably advisable to avoid empty commits using: `git cherry-pick <commit-sha> --empty=drop`


If you create a `feature` branch and someone pushed changes to the main branch of the repo, there's a couple of options to resolve this.
- rebase
- cherry-pick


Cherry-picking is a powerful feature of git, however it's important to understand when it's useful and possible alternatives. A few scenarios in which a cherry-pick is appropriate are: 
- Pulling a commit or sequence of commits from a stale feature branch to an active one.
- Bug hot fix which can be committed independently from the work on a feature branch.

