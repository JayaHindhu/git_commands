1.What is version control system? 

A version control system is a software that tracks changes to a file or set of files over time so that you can recall specific versions later. It also allows you to work together with other programmers. The version control system is a collection of software tools that help a team to manage changes in a source code. It uses a special kind of database to keep track of every modification to the code.

2.What is Git? 

Git is an open-source distributed version control system. It is designed to handle minor to major projects with high speed and efficiency. It is developed to co-ordinate the work among the developers.

3.What is Repository? 

In Git, the repository is like a data structure used by VCS to store metadata for a set of files and directories. It contains the collection of the files as well as the history of changes made to those files. Repository in Git is considered as your project folder. A repository has all the project-related data. Distinct projects have distinct repositories.

4.What is Git bash? 

Git Bash is an application for Microsoft Windows environments which provides an emulation layer for a Git command line experience. Bash is an acronym for Bourne Again Shell.A shell is a terminal application used to interface with an operating system through written commands. Bash is a popular default shell on Linux and macOS. Git Bash is a package that installs Bash, some common bash utilities, and Git on a Windows operating system.

5.What is Github? 

GitHub is a Git repository hosting service. GitHub also facilitates with many of its features, such as access control and collaboration. It provides a Web-based graphical interface.It hosts source code of your project in the form of different programming languages and keeps track of the various changes made by programmers.

6.What is branch in git? 

In Git, branches are a part of your everyday development process. Git branches are effectively a pointer to a snapshot of your changes. When you want to add a new feature or fix a bug—no matter how big or how small—you spawn a new branch to encapsulate your changes.

7.What is commit in git? 

It is used to record the changes in the repository. It is the next command after the git add. Every commit contains the index data and the commit message. Every commit forms a parent-child relationship. When we add a file in Git, it will take place in the staging area. A commit command is used to fetch updates from the staging area to the repository.

8.What is a merge conflict? 

A merge conflict is an event that takes place when Git is unable to automatically resolve differences in code between two commits. Git can merge the changes automatically only if the commits are on different lines or branches. (or) A conflict arises when two separate branches have made edits to the same line in a file.

9.Where is conflict? How to identify? 

We can see some strange settings

HEAD ======= >>>>>>>BRANCH-NAME To see the beginning of the merge conflict in your file, search the file for the conflict marker <<<<<<<. When you open the file in your text editor, you'll see the changes from the HEAD or base branch after the line <<<<<<< HEAD. Next, you'll see =======, which divides your changes from the changes in the other branch, followed by >>>>>>> BRANCH-NAME. By this symbols we can identify conflicts.

10.How to resolve the conflict? 

The most direct way to resolve a merge conflict is to edit the conflicted file. Open the file in your favorite editor.Lets simply remove all the conflict dividers.Once the file has been edited use git add filename to stage the new merged content. To finalize the merge create a new commit by executing it. Git will see that the conflict has been resolved and creates a new merge commit to finalize the merge.

11.what is the difference between git fetch and git pull?

In Git fetch it will just fetch all the changes in the remote repository (Github) and move the origin/master pointer to HEAD. Meanwhile your local branch master will keep pointing to where it has.
In Git pull, it will do basically fetch and merge any new changes to your master branch and move the pointer to HEAD.
So, git pull=git fetch + merge.


Basic Git Commands

git clone repository_url - The git clone is a command-line utility which is used to make a local copy of a remote repository. It accesses the repository through a remote URL. (or) This will give the copy of the repository with default branch.

git init - The git init command is the first command that you will run on Git. The git init command is used to create a new blank repository. It is used to make an existing project as a Git project. Several Git commands run inside the repository, but init command can be run outside of the repository.

git branch - List all of the branches in our repository.Add argument to create new branch with the name.

git checkout -b branch_name - Create and checkout a new branch named.Drop the -b flag to
checkout an existing branch.

git add filename - This adds new file and also modified files.

git add* - The git add command adds new or changed files in your working directory to the Git staging area.

git add. - To add all the files from the repository, we run the add. command

git status - This shows the track and untracked files (or) this shows modified and newly added files.

git diff - lists out the changes between your current working directory and your staging area.

git commit -m "message" - Commit staged changes to local repository. The -m option of commit command lets you to write the commit message on the command line.

git push origin branch_name - Pushing the codes from our local system to github server.

git pull origin branch_name - it will fetch the remote branch and then merge it into your current local branch.

git fetch --all - It will only track the remote branches and track local branches that track remote branches respectively. Run this command only if there are remote branches on the server which are untracked by your local branches. (or) It fetches all metadata about repository from remote to local.

git merge branch_name - This command merges the codes of one branch to another. (or) Merge remote branch into current local branch.

git config --list - The git config list command will show all Git config properties throughout all of the variously scoped Git files.

git remote -v - Git remote supports a specific option -v to show the URLs that Git has stored as a short name. These short names are used during the reading and write operation. Here, -v stands for verbose.

git config --global user.email"youremail" - Define author email to be used for all commits by the user.