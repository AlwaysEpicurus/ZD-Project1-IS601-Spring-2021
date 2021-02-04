# Checkout

## Definition
* Lets the user navigate between the branches that are created with git branch [1]
* Checking out a branch updates the files in the working directory to match the version stored in that branch, and tells Git to record all new commits on that branch [1]


## Examples

This will make the specified branch the new HEAD branch.
```
git checkout <branch>
```

This will create a new branch, <branch>, and then makes it the new HEAD branch.
```
git checkout -b <branch>
```

Sources:
* [Git Checkout](https://www.atlassian.com/git/tutorials/using-branches/git-checkout)

[Link to Previous Page](/terms.md)