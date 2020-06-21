Git tracks the files it knows about in its database.  In other courses, we'll talk about the states of files -- both tracked and untracked -- but if you make a change to a file that Git is tracking, it will not allow you to switch to another branch until you either commit your latest changes, abandon your changes, or temporarily stash your changes.

This is important to understand because you might be working on an exercise assignment and you're modifying the code files.  You want to take a peek at the solution branch to see how I solved the exercise.  You attempt to change branches, but Git prevents you from changing branches.  Why?  Because you must either: commit your changes, abandon your changes, or stash your changes.  Remember: if we change branches, Git will delete all of the files in the directory it is tracking and replace them with the version of the files stored in the latest commit on the branch you're requesting.

In this video, I'm only going to show you how to commit your changes because it is the safest option.  In other words, if you do what I show you here, you'll never lose any code, and any new files you add will be tracked from that point on as well.

Let's walk through this scenario.

# Commit scenario

```
git checkout master
```

We'll make a change to the file.  Now, let's try to change to the solution branch.

```
git checkout solution
```

Notice the error message.

```
git status
```

Let's commit the change:

```
git add .
git commit -m "Working on exercise"
git status
git checkout solution
git checkout master
```
