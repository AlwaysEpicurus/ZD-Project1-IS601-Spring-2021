# Merge

## Definition

* At the most basic level, the Merge command allows you to merge two or more local but divergent branches.

* The Merge command merges the branches with simliar histories. 

* If changes between each branch conflict the merge will fail.

* Merging uses the same steps as the push. change -> stage -> commit -> execute.

## Examples

Merge Process
```
# Create New Branch and move Head to that branch
git branch -m NewBranch
git checkout NewBranch

# Then add your changes, updates, etc.
git add NewFile
git status
git commit -m 'New Stuff and Changes'

# Then merge teh new branch with the master
git checkout master
git merge New Branch
```

```

## Sources

* Atlassian Bitbucket "Git Merge" (https://www.atlassian.com/git/tutorials/using-branches/git-merge)

* Tower "Git Commands: git merge" (https://www.git-tower.com/learn/git/commands/git-merge/)

* Tower "Git FAQ: git merge - How to Integrate Branches (https://www.git-tower.com/learn/git/faq/git-merge-branch/)

* GitHub Docs "mege" (https://docs.github.com/en/github/getting-started-with-github/github-glossary#merge)

* Stake Abouse "Git: Merge Branch into Master" (https://stackabuse.com/git-merge-branch-into-master/)
