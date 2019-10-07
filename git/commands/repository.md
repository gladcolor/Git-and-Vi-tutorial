# Repository

# What is repository
Respository is the set of files, such as code files, tracked by Git. The changes of these files are recorded by Git and can be restored.

# Why repository
Repository is the object managermented by Git. Basicaaly, a repository is the archive of a project.

# How repository
A repository can be built from the remote server or the local machine. 

For beginers, the most common method is create a repository from github.com and clone it to the local machine.  

Another method is creating a new foler in the local machine and let Git track the changes of files in this folder. 

```Git
git init folder_name
```

However, Git would not track the files automatically unless you tell it which file should be tracked. You can track files using these two commands after you change the present working directory in the comannd (shell) window.


Track a specific file:
```Git
git add filename
```

Track all the files:
```Git
git add --all
```