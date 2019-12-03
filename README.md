# GitHub Tutorial

_by Perla Lopez_

---
## Git vs. GitHub
**Git** is all about version control so it qllows you to manage the history of all your files and folders. In other words, it allows all the changes we make be saved and we're allowed to see the history of the changes.
**Github** is a website where it allows you to update your git repository where other users can view your work
and collaborate something to your work by forking and cloning it.

---
## Initial Setup
Steps to creating a github account:

1. Go to github.com
2. Click sign up and fill out your personal information

After you've filled in your personal information and signed up to github we can now move on to setting up your ide.

1. Go to ide.cs50.io
2. Then go to the following link [github](https://github.com/hstatsep/ide50) and follow further
directions given

When setting up our ide we are basically working on setting up an SSH key. We need an SSH key to conect with github, when using Github we need to let the computer know your username and password every single time.
With an SSH key it helps the github repository know that it's you accesing your code not needing to put your username and password each time you go on github.

---
## Repository Setup
Initializing a new repository:
1. Go to [github.com](github.com)
2. Then sign in with your github account
3. Then click on the far right corner there's a button that is "+" it wil give you an option of making a new repository and sso you click on that
4. It will then take you to a new page where it says "repository name", you will then go ahead and give your new repository a name
5. After that is done at the bottom of the page it says "create create repository" and you click on that
6. Then you copy whatever is the second section that says "…or push an existing repository from the command line"
7. Next you make sure you're in the root directory and you do

   `git remote add origin git@github.com:username/nameofrepo.git`

    `git push -u origin master`

Doing the top command will make will push any changes from the local branch to the remote branch.

Your new repository will then show on your ide and when to go to the repository you must **cd** into it making sure you're not in the root directory.
After doing so you should do **git init** to initialize it and whenever you make any changes in it make sure to **git add** and **git commit -m "message"** to make
that any changes can be saved on stage.



---
## Workflow & Commands
* `git status` ~ Allows you to check what you've done like what you've added, commited, or pushed
* `git add .`  ~ Adds all changes in the file to the stage so that you're able to commit
* `git add "file name"` ~ Adds a specific file to the stage and commits changes.
* `git commit -m "message"`~Saves the changes in the stage area
* `git push`   ~ Pushes any changes made to certain branch allowing them to save in that certain branch in
your repository in github

---
## Rolling Back Changes
* When wanting to undo something you committed you can simply do as shown below, it is used for undoing changes that you have already committed in the repository.

    `git revert HEAD`

  * When using this command you do **git log** to see your latest commit and then after there will be a set of numbers and letters. You will then copy those set of numbers
    and letters and go to your repository and do **git revert HEAD** in which **HEAD** stands for the set of numbers and letters. This will then undo any changes you have
    commited.

* Using the command below gives us the ability to discard any changes we've made by removing them so in any case that we want to remove anything we've added or changed in our program.

    `git checkout “file name”`

    * When using this command you should do **git status** to see if you have anything committed at the moment to discard so if it is green then you can use the command above undoing the commit you've done.

* When wanting to remove your latest commit you can use the command below.

  `git reset HEAD`

    * When you want to use this command it's because you want to undo a commit in a certain file. When you do **git status** it shows if you committed any of your changes or not,
    when doing so if it shows that there's anything committed then you can use the command above to undo the changes.


* The command below undoes anything that was recently commited and added.

    `git reset --soft HEAD~1`

    *You can use this command to undo any changes that have been committed or added after checking your status to see if you have anything committed.

These commands are very useful because in case we add or commit something in the wrong repository we're able to undo and if we
add any code that we want to change then all we can do is undo letting us fix our mistakes.
