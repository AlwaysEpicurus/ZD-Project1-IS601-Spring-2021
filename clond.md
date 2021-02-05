# Clone

## Definition

* The clone command allows you to place a copy of a remote repository on your local drive.
* It also maintains a connection between the original (remote) repository and your cloned (local) repository so you can easily keep both in sync using other git commands.  

## Examples

Clone a remote repository
```
git clone (repository URL or SSH key)
```

Clone a remote GitHub respository using a repostiory URL
```
git clone https://github.com/username/repository.git
```

Clone a remote GitHub respository using a SSH key
```
git clone git@github.com:username/repository.git
```

If you want to clone a repostiory to a specific local folder
```
git clone <repot> <localdirecotry>
```

## Sources
* Atlassian Bitbucket "git clone" https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-clone
* GitHub Docs "clone" https://docs.github.com/en/github/getting-started-with-github/github-glossary#clone

