# GitFlow

## What is it?

* Development of projects with the use of parallel branches -- main branch and development branch
    * Main branch: branch that was tested and will be released when ready to do so [1]
    * Development branch: branch where all features reside and all tests are performed on [1]
    * In this workflow, the development branch can be merged with the main branch when all issues (bug, fixes) have been resolved, and all tests have been performed [1]
* Overall, it is good for software projects that occur in stages
    * Certain features can be developed simultaneuously, and once those are complete they can then be merged into the develop branch, and then finally the main branch
    * It is important to pay attention to the structure of the project, as this workflow can become convuluted with the number of features, hotfixes, and releases branches

## What are the benefits to using it?

* Parallel Development Improves Productivity
    * The ability to have multiple branches that work on different parts of the project is beneficial, as nothing gets mixed up. Each type of branch has a role to play in ensuring productivity is high, and the product is polished
    * The ability to have multiple users work on different aspects of the project without negatively affecting each other's work is important for productivity [2]
    * Once a part of the project is completed, it is then merged back into the develop branch. The develop branch can be thought of a staging area, where completed features wait until they are released to the main branch.
      This way, everything is up-to-date and there are no conflicts between features. [2]
* Collaboration + Communication
    * The feature branch gives the flexibity for multiple users to work on a feature simultaneously [2]
    * The feature branch does no harm to the develop or main branch (unless deemed ready to merge). In this way, the developers are free to make changes as they see fit, and they are able to see what work has been done.
* Proper Staging Area
    * As stated previously, the develop branch is a staging area for completed features that are waiting to be released [2]
    * This gives the main branch the most recent work that has been finished [2]
* Management of Emergency Fixes
    * The hotfix branch allows for developers to fix a severe bug without worrying about the main branch being affected

## Basic Examples and Commands (main, develop, feature) 

* These first commands create the develop branch locally (1st line), in which features branch off of and ultimately merge together to form a complete product. The second line
pushes the newly created develop branch to the server [3], which thus begins the workflow.
```
git branch develop
git push -u origin develop
```

* Executing the following command will create the develop branch on an already existing repository [3]
```
git flow init
```


* Below are two differing methods of creating the feature branch. [3] The former first checks the develop branch, and from here creates the feature_branch, and then checks that. It still performs the same task, but is rather long.
The latter is more concise, as simply typing out this command on the develop branch creates the desired feature_branch, and checks it.
```
git checkout develop
git checkout -b feature_branch
```
```
git flow feature start feature_branch
```


* Merging each complete feature is as simple as starting one with the proper commands. [3] The former again checks the develop branch, and from here merges the changes from the feature_branch together with the develop branch
to obtain the latest changes. It does the job, but the latter provides a simpler approach. Simply typing out the latter command does the exact same thing as the former, but in one line. It checks the feature_branch
for any changes, and then merges it into the develop branch.
```
git checkout develop
git merge feature_branch
```
```
git flow feature finish feature_branch
```


Sources:
[HOW TO USE GIT TO IMPROVE YOUR DEVELOPMENT PROCESS](https://www.popwebdesign.net/popart_blog/en/2017/11/how-to-use-git-to-improve-your-development-process/)
[Introducing GitFlow](https://datasift.github.io/gitflow/IntroducingGitFlow.html)
[GitFlow Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)