You'll use Git to download my files from Github, or rather, you'll "clone a repository" from Github.

A repository is a database of all the files in a folder.  This usually includes all files that comprise a single project source like code files, configuration files, license files, and other text files that have instructions or other information.  Sometimes, this might include other files like images.

A repository contains the current snapshot of the files at a single point in time, as well as all the previous snapshots.

You will need a local copy of the repository, and to do that you'll perform a "clone" operation.  We'll do that in an upcoming video.

But to prepare, I want you to create two folders on your hard drive:

- c:\bobtabor ... this is where you'll clone my repositories.  Sometimes, you'll simply refer to my code, other times you will make changes to my code.
- c:\source ... this is where you'll create new C# projects.

In this way, you'll be able to follow along with me while I write code.  But if you get stuck, you can clone my repository.  Since it will be in a different directory, you will be able to switch back and forth between my code and your code without overwriting one or the other.

Windows wants you to put all of your work in a User's directory.  In my case, that's:

c:\users\bobta\

However, I always prefer to work against the root of the drive.

```dos
cd ..
cd ..
mkdir bobtabor
mkdir source
dir
```

