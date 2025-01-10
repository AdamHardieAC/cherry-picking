### Notes

Using git cherry-pick <branch-name>, will take the head commit of the branch.

- Cherry picking a merge commit causes some complications, such as an empty commit message without the merge changes causing an empty commit.
- It's probably advisable to avoid empty commits using: git cherry-pick <commit-sha> --empty=drop