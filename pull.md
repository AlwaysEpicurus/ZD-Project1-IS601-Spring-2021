# Pull

## Definition

* The Pull command allows you to update your local repository with any updates from its parent (remote) repository.

* It is similar to the Feth command in that it downloads updates (refs & heads) from the remote repository, then like the Merge comand it  merges the download into the local branch. 


## Example

Git Pull - Fetch a specific brnach and merge with local repository
```
git pull <remote>
```

Git Pull Rebase - Puts most recent commit on top
```
git pull --rebease <remote>
```

Git Pull Verbose - Gives you additional details about the Pull operation
```
git pull --verbose
```




## Sources
* Atalssian Bitbucket "Tutorials: git pull" (https://www.atlassian.com/git/tutorials/syncing/git-pull)

* GitHub Docs "GitHub glossary: pull" (https://docs.github.com/en/github/getting-started-with-github/github-glossary#pull)


