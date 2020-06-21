A repo contains snapshots of all the files at a moment in time.  These snapshots are known as commits.

Each commit stores several things:
- The snapshot of all the files
- The name and email address of the person who created the commit
- The date and time of the commit
- The parent commit

By storing the parent commit, it's possible to trace a path back from the current version of the files to the first version of the files, and you can trace the history of the project.  Storing the parent is also a key piece of information that allows Git to store the snapshots, or commits, very efficiently, only storing the changes, and assembling everything back together seemlessly so that you never have to think about it.

Git has a flexible system of branches which allow the development of the software to diverge.  This is useful when you want to maintain two (or more) versions of your code: one version which represents the version that is stable and used by your customers, and a second version of the source files where you fix bugs, or add new features.  At some point in time, once you've fixed bugs or added new features, and you've tested the changes and you're sure they work, you can merge those changes together.

But to easily keep track of these two paths, you can refer to them by their branch name.  This allows you to switch back and forth.  A branch is simply a bookmark to the latest snapshot of a divergant development effort.  Once you merge the changes you made into the main, or master, branch, you can delete the branch if you don't anticipate any further changes.  Branches are intended to be temporary.  Git anticipates you'll delete branches once you no longer need them -- once you've merged the commits into another branch.

I tell you all of that to say this: branches will help me give you multiple versions of the source code as I record the videos.  I might provide a "before" and "after" view of the code.  Or, I might provide source code exercises or challenges on the main or master branch, and you can peak at the solution to the exercise or challenge on a different branch.

To illustrate that, `my-first-repo` has a second branch.  To switch to that branch, do the following:

```
git checkout solution
```

If you have Visual Studio Code open, you can see that the file changed.  Git looked in its database and pulled out the snapshot that the solution branch is pointing to.  Behind the scenes, Git basically deleted everything in the working directory and replaced it with the contents of the snapshot.  Once Visual Studio Code realized the file is was looking at has changed, it refreshes.

To switch back, use the following command:

```
git checkout master
```

