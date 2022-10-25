
<h1 align="center">Hi there, I'm <a href="https://github.com/Lexuse/" target="_blank">Tarala Aleksey</a> 
<img src="https://github.com/blackcater/blackcater/raw/main/images/Hi.gif" height="32"/></h1>
<h3 align="center">I am a GeekBrain student on a developer course</h3>

As part of my homework at the Git seminar, I wrote a short tutorial on the most important functions
<hr>

<div>
<h10 align="right"> Git distributions for Linux and POSIX systems are available from the official Git SCM website. <a href="desktop.github.com" target="_blank">GitHub Desktop</a>
</div>

<hr>

>### Initial setup
*git config --global user.name "[name]"* - Sets the name that will appear in the author field of commits you make

*git config --global user.email "[email]"* - The email adress that will be displayed in the information about the commits you make

>### Creating repository

*cd ~/Desktop*

*mkdir myproject*

*cd myproject/*

*git init [name of project]* - creates a new local repository with given name

*git clone [url-adress]* - downloads a repository along with its entire change history

>### Push a local repository from you computer to GitHub
*git remote add origin https://github.com/[your-username]/[repository-name.git]*

*git push -u origin master* 
>### Add a file to repository
Git notices when you add or modify files in the folder containing the Git repository but doesn't track the file unless instructed. Git saves the changes only for the files it tracks, so you need to let Git know you want to track changes for a specific file.

*git status* - You can check which files Git is tracking by running

*git add [filename]* - Git notifies you if you have any untracked files. If you want Git to start tracking a file, run the following command:

>### Unstage Files on Git
Working with Git usually involves adding all the files to your index to prepare them for a commit. If you want to remove some files from the index before committing, you have to unstage the files in Git.
One way to unstage files on Git is to run the git reset command. The syntax is:

*git reset [commit] -- [file_path]*

You can also use the rm command to unstage files on Git.

*git rm --cached [file-name].*

>### Create a Commit
After adding the specified files to the staging environment, instruct Git to package the files into a commit using the git commit command. Git then stores that file version. You can review the stored version at any given time.

*git commit -m "Notes about the commit"*

>###  Undo Last Commit
Use the revert and reset commands to undo changes and revert to a previous commit.
To undo a published commit, use the following syntax:2

*git revert [hash]*

A hash is a code that identifies each commit. Obtain a commit hash by running:

*git log*

Or

*git log --oneline*

>### Branch

The first branch in a git repository is called master, and it is the primary branch in a project.

Creating a new Git branch means creating a copy of the project from a specific point in time. Branches in Git allow users to make new features without applying the changes to the main branch while the feature is in development.

The common method for creating a new branch is by running:

*git branch [new_branch_name]* -just create a branch but stay in the existing one

*git checkout -b [new_branch]* - go directly to the created branch

*git checkout master* - go to the master branch

*git branch -d [new_branch]* - remove existing branch

*git push [remote_project] --delete [branch_name]* - delete a remote Git branch

*git branch -m new-name* - rename branch

>### Remove a Git Remote
A git remote is a connection to a repository hosted on a remote server – GitHub, BitBucket, GitLab, or any other remote location.
However, over time, the remote repository may move to another host, or a team member may stop working on the project. The remote in question is then no longer needed.

*git remote remove [remote name]* -  One of the ways is to delete a remote

>### Git Merge
Git merge unifies multiple commit sequences into a single commit. It can combine two branches, thus integrating the independent development lines into a single branch.

After merging two branches, Git updates the current branch to reflect the merge, but the target branch isn't affected. That means you have to use the git branch -d command to delete the obsolete target branch.

For example, you may want to merge a new feature branch into the main branch. Follow the steps below:

1. Run the git status command to ensure that HEAD is pointing to the correct merge-receiving (master) branch. If it is not, run git checkout master to switch to the master branch.
2. Run git fetch to pull the latest remote commits and git pull to ensure the main branch has the latest updates.
3. Run git merge X where X is the name of the branch you want to merge into the receiving branch.
>### Resolve Merge Conflicts
Merge conflicts usually occur when multiple developers work on the same code of a project or when they work with several development branches. Git merge warns the user about these conflicts
>### Create a Pull Request
Create a pull request (PR) to inform a repository owner that they should review the changes you've made to their code. Then the owner can approve the pull request and merge the changes into the main repository.

If you are the co-owner or owner of a repository, you don't have to create pull requests to merge your changes. However, you can still do it to keep track of your feature updates and history.
>###  Synchronize Changes on GitHub and Locally
When you merge changes on GitHub, they don't appear automatically in your local repository. You have to pull the changes to your local repository to see the updates.

*git pull origin master* - Synchronize your local repository with GitHub