In this video, we'll configure git.  During installation, many options were configured.  But we'll tell Git who we are now so that later when we create a snapshot of our files, or rather, a "commit" in Git terminology, it will not interrupt us and force us to configure our name and email address first.

To view the current configuration settings:

```cmd
git config --list
```

To configure our name and email address, we'll run the following commands:

```cmd
git config --global user.name "Bob Tabor"
git config --global user.email obviously@fake.com
```
These settings are used when you want to take a snapshot of changes you've made to the files.  I'll talk more about that in the next few lessons.

Now that we've made the changes, we'll re-run the commad to make sure our settings are correct:

```cmd
git config --list
```