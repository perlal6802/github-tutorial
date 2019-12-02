# GitHub Tutorial

_by Perla Lopez_

---
## Git vs. GitHub
**Git** is all about version control so it qllows you to manage the history of all your files and folders. In other words, it allows all the changes we make be saved and we're allowed to see the history of the changes.
On the other hand **github** is the git repository where it allows you to using git.

---
## Initial Setup
Steps to creating a github account:

1. Go to github.com
2. Click sign up by filling out your personal information

After you've filled in your personal information and signed up to github we can now move on to setting up your ide.

1. Go to ide.cs50.io
2. Then go to the following link [github](https://github.com/hstatsep/ide50) and follow further
directions given

We need an SSH key because it allows us to make our code public allowing others to see our code and it allows you to clone and pull other code that is public to us.


---
## Repository Setup

---
## Workflow & Commands
* `git status` ~ Allows you to check what you've done like what you've added, commited, or pushed
* `git add .`  ~ Adds all changes in the file to the stage so that you're able to commit
* `git add "file name"` ~ Adds a specific file to the stage and commits changes.
* `git push`   ~ Pushes any changes made to certain branch allowing them to save in that certain branch in
your repository in github
* `git commit -m "message"`~Saves the changes in the stage area
* 



---
## Rolling Back Changes
When rolling back on changes there are quite a few commands that we can use but they're all used for something specific.
For example,

    `git reset --soft HEAD-1`

We can use this if we accidently commit something we didn't want to, this command lets us undo the commit by removing it.

There's also

    `Git checkout “file name”`

This gives us the ability to discard any changes we've made by removing them so in any case that we want to remove anything we've added or changed in our program.

Lastly there's .

    `git reset HEAD~1`

This command undoes anything that was recently commited and added.

These commands are very useful because in case we add or commit something in the wrong repository we're able to undo and if we
add any code that we want to change then all we can do is undo letting us fix our mistakes.
