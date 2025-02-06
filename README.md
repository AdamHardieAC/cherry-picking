### Git cherry-pick
Repo intended for learning the in's, out's and intricacies of cherry-pick.

### At a glance
Given one or more existing commits, apply the change each one introduces, recording a new commit for each. This requires your working tree to be clean (no modifications from the HEAD commit).

When it is not obvious how to apply a change, the following happens:

    The current branch and HEAD pointer stay at the last commit successfully made.

    The CHERRY_PICK_HEAD ref is set to point at the commit that introduced the change that is difficult to apply.

    Paths in which the change applied cleanly are updated both in the index file and in your working tree.

    For conflicting paths, the index file records up to three versions, as described in the "TRUE MERGE" section of git-merge[1]. The working tree files will include a description of the conflict bracketed by the usual conflict markers <<<<<<< and >>>>>>>.

    No other modifications are made.

sequence commit 1
sequence commit 2
sequence commit 3