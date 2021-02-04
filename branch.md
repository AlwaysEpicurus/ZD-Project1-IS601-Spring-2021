# Branch

## Definition

* A fork is a copy of a repository, and forking a repository allows a user to make changes without affecting the original project [1]
* Represents an independent line of development, where users can then continue the edit/stage/commit process [2]

## Examples

Lists all of the branches in your repository.
```
git branch
```

Creates a new branch called <name>, but does not check it out. 
```
git branch <name>
```

Deletes the branch <name>, and is considered a safer operation in that it prevents you from deleting the branch with unmerged changes. [2]
The -D option can also be used, but will delete everything with no further warning.
```
git branch -d <name>
```

Renames the current branch to <newName>.
```
git branch -m <newName>
```

Lists all the remote branches the user has.
```
git branch -a
```

Sources:
* [Git Branch](https://www.git-tower.com/learn/git/commands/git-branch)
* [Using Branches](https://www.atlassian.com/git/tutorials/using-branches)

[Link to Previous Page](/terms.md) 

