# Repository


## Definition

* Virtual storage of your project [1]
* Allows you to save versions of your project, which you can then access at any time [1]
* How to initialize a repository:
    * "git init"
    * Creates a new Git repository
    * Can convert an existing project to a Git repository or initialize a new, empty repository
    * Creates a .git subdirectory in the current working directory

## Examples


Once the user has changed into their desired project subdirectory, using **git init** will create a new, empty Git repository.
This will add a .git subdirectory into the current working directory, and the user can thus begin to record revisions of their project.
```
git init
```

This will create a new, empty Git repository in the directory the user specifies. Similar to above, the this directory will only have the 
.git subdirectory, and nothing else.
```
git init <dir>
```

Sources:
[1] [Setting up a repository](https://www.atlassian.com/git/tutorials/setting-up-a-repository)



[Link to Previous Page](/Section3.md) 