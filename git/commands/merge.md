# What is Merge?
Once you have fixed all the bugs or added new features in branches, you face the problem how to merge these changes into the master branch. Merge command gives you the power to do that. It will put the individual changes together to form a final version.

# Why Merge?
Branch command divert the version to new direction, and there is so many discrete directions separate from the master branch. Finally, they need to converge together. Merge command is the tool to lead these branches into the final point.

# How to Merge?
Merge command work with two branches, and you need to checkout the master before merge the targeted branch.

```git
git checkout master
```

Then merge the branch:

```git
git merge checkout_cmd
```

This is an example to merge a branch name "checkout_cmd" to the master branch.
![merge](/git/img/merge.jpg)



