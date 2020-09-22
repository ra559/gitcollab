# What is Git?
Git is a version control system that records changes to a file or set of files over time. Version control systems allow developers to:
* Revert the entire project back with the use of snapshots,
* Compare file changes
* See user's last modification
* See who/when and issue was introduced
* Easy file recovery in case of errors or emergencies
## Note:
Nothing beats reading the manual. So if you want to, Gits documentation can be found here:
https://git-scm.com/doc

## Installing Git
* Windows:
  * Download from here: https://git-scm.com/download/win
* Mac:
  * Download from here: https://git-scm.com/download/mac
* Linux:
    * Debian/Ubuntu:
      * **sudo apt install git-all**
    * RHEL/CentOS/Fedora:
      * **sudo dnf install git-all**
    * Arch:
      * **sudo pacman -S git**
## Basic Git Commands
* git **init**: Use this command to initialize a local repository.
* git **clone**: Use this command to bring (download) a repository from github to your local machine.
* git **add**: Use this command to track changes to your files.
* git **commit**: Use this command to save your files in git.
* git **status**: Use this command to check the status of a working tree.
* git **push**: Use this command to save your committed changes to a remote repository (github/bitbucket/gitlab)
* git **pull**: Download changes from a remote repo to your local repo.
* git **--version**: Use this command to check the version of git installed in your system.
* git **config --global [object]**: Use this command to change gits global configuration.
* git **rm cached [file or . for all]**: Use this command to remove all cached information.
## Note
To demonstrate how to use all of this commands, we will create a simple website with git and github.

## Creating the site
To create the site we use:
**git init demoSite**
This command will create a directory and initialize the directory as an empty git repository.
[image goes here]

Now we can create a couple of files to get started with the HTML. If you are using an IDE like VS Code you can open the terminal from vs code and create the files there. 
[gif here]

## Adding more files and directories
To this website we are going to add a directory for assets and a directory for css. In the terminal, use the mkdir and touch commands to create the directories and files. Then we are going to use the following git commands to commit these changes.
* Use the **git add .** command to add all the files to the repo.
* Use the **git commit -m "added css and assets directories"** the -m flag is for message which is required for committing changes.
**WARNING!!!**
Make sure to add your name and email address to your git installation. Otherwise git will complain about  it.
Use the commands:
* git config --global user.name github username here
* git config --global user.email github email here
If you do not have a github account, now is a good time to create one.
[image here]

## Adding changes and committing
Now lets add some content and practice some commits. Since this is a dummy site, I added dummy content using VS Code lorem ipsum generator extension.
To commit these changes use:
* git add . 
* git commit -m "added more content"

At this point it is a good idea to check on the status of our git repo. We do this we the command:
* git status

[image here]

Now lets add a little css to the styles file, add the changes but instead of committing let's see what the status command outputs. As you can see bellow, when changes are made the status command shows what is pending for committing.

## Creating a fork of the site
Sometimes developers need the entire repository for experimentation, use it as a base for another project, or fixing a bug. In this cases, developers can fork the repository and work on it independently of the original repository. If the developer fixed a bug they can then submit a pull request to have the project owner merge the the changes.

To fork a repository, we use the **git clone** command. Later on we will see an example of how to use the git clone command.

## Working with Branches
Let's assume that our dummy website requires a separate page and you have assigned the development of this page to another team member. The best way to work on this page is by creating a branch. A branch is separate from the master and as such the changes made to the branch will not affect the master until a merge is done. To create a branch use the command:
**git branch formpage**
This command will create a branch but it will not switch your working environment to such branch. For that we use the command:
**git checkout formpage**.
### Tip:
You can use the command **git checkout -b formpage** to create a branch and switch to that branch at the same time.
[image here]

To change between branches use the checkout command.
* git checkout master
* git checktout formpage
[gif here]

## Merging work
To merge work means to combine a particular branch with the master branch. For example, to merge the formpage branch to the master branch first change to master branch and then use the command:
* git merge formpage
[insert image here]



# What is Github?
**_Note:_** In this section we will be using the commands:
* git pull
* git push
* git remote Add/Remove/Show

GitHub, Inc. is a hosting service for software development and version control using Git. Github provides	all the benefits of Git plus additional features of the Github platform. GitHub offers its basic services free of charge while its more advanced features are commercially available. Some of these features are bug tracking, feature requests, and task management

To join github go to https://github.com/. Once you have created an account you can create a repository directly in Github and start working.
[insert image here]


## Creating a repository for the website
click on the + sign located in top right corner and select **"New Repository"**. Now, to push our git repository of the dummysite to Github, we use the git remote commands: 
* git remote add origin https://github.com/robertalberto350/dummysite.git
* get branch -M master
* get push -u origin master

**_NOTE_**
Make sure to either setup SSH keys or set up vs code github extension. Or ignore this if you rather enter your username and password in every push 
* To setup SSH keys see these links:
  * https://docs.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account
  * https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh
* To setup SSH in VS Code see this link:
  * https://code.visualstudio.com/docs/editor/github



