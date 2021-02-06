# Commit

## Definition
* Captures a snapshot of the project’s currently staged changes [1]
* “git add” precedes the commit, where “git add” puts any potential commits in the staging area

## Examples

Use **git add** to stage the changes of test.txt for the next commit. Then, **git commit** will put the new changes
in a new commit object.
```
git add test.txt
git commit -m "Fixed typo in test.txt"
```

Use -a when you have a lot of changes you want included in the next commit. With this option, you do not need to include the **git add** command.
```
git commit -a -m "Added fixes to two files"
```

Use --amend when you need to fix a typo in a previous commit's message or forgot to add a necessary change.
The following example corrects the last commit by putting in a new commit message
```
git add amended_file.html
git commit --amend -m "Amended file with necessary typo changes"
```

Sources:
* [Git Commit](https://www.atlassian.com/git/tutorials/saving-changes/git-commit)

[Link to Previous Page](/Section3.md) 
