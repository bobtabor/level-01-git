A repository contains the current snapshot of the files at a single point in time, as well as all the previous snapshots.

To view the files or make changes in a repository, or "repo", you will need a local copy of the repo, and to do that you'll perform a "clone" operation and point to a shared repository like Github.

Github is simply a shared repository, meaning that I can create a repository on my local computer, then push it to Github to make an exact copy there.  At that point others can clone the repository, contribute to it by making their changes on their local computer, then attempt to push their change to the central Github repository.  We'll talk about that workflow in another series.  The key idea is that Github is a Git server that allows anyone to push a local repo to a centralized store, and others can clone that repo.

Let's do that now.

```
cd bobtabor
git clone https://github.com/bobtabor/my-first-repo
dir
code .
```
In this case, I have just one file in my repo.  I could have dozens or hundreds of files if needed.

You might be wondering "If Git stores every snapshot of the folder, then were is it hiding?"

You cannot see Git's "database" by using "dir" from the command prompt.  It might be easier to use Windows Explorer.

Here you can see the .git folder.  Git's "database" is just a series of ascii text files, some binary encoded files, and lots of folders.  At some point, we'll explore Git's internals so you can understand how it works under the hood to store all that information efficiently.  For now, I recommend you do not delete the .Git folder unless you want to completely blow away all the code you cloned, as well as all the changes you made but haven't pushed back to the shared repository on Github.

