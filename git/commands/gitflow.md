
# GitFlow

## What is GitFlow?
GitFlow is a software developmental pattern to control versions of master, develop, release, feature branches, and so on. Based on Git and the idea of GitFLow, a software development team will have a clear workflow to control various versions in the life circle of software.

Before digging into the details, the following chart is helpful to give you a big picture of GitFlow. GitFlow uses these braches:

**Master**: The main branch of the software. It is the achive of the development work.

**Develop**: Developing version will be branched off from develop branch.

**Feature branches**: Develope major features for the next release in this branch. Feature branches are branched off of the develop branch, and finished features and fixes are merged back into the develop branch when they’re ready for release. New development (new features, non-emergency bug fixes) are built in feature branches:

**Release branches**: When it is time to make a release, a release branch is created off of develop. The code in the release branch is deployed onto a suitable test environment, tested, and any problems are fixed directly in the release branch. 

**Hotfixes**: Used for emergecy bug fix.
 
![](https://nvie.com/img/git-model@2x.png)
[Chart: Vincent Driessen](https://nvie.com/posts/a-successful-git-branching-model/)

## why GitFlow?

Like other industrial fields, most software developments need a team work together to produce qualified commerial products. GitFlow is a pragmatic method to organize and trace the production activities. For new teams and novices in programming, GitFlow is a reliable branch model. 


## How to GitFlow?
Basically, GitFlow is a method of version control, and it reflects the management on software development. Git serves as a basic tool here, but other similar version control tool can be also applied. GitFlow does require the fluency of Git, however, software engineering is a prerequisite. The careful arrangment of the develop, feature, and other branches is the key to setup a useful GitFlow.  
