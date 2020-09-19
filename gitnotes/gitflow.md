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
Now lets add some content and practice some commits. Since this is a dummy site, I added dummy content using VS Code lorem ipsum generator extention.


## Creating a fork of the site

## Working with Branches

## Merging work


## What is Github?
GitHub, Inc. is a hosting service for software development and version control using Git. Github provides	all the benefits of Git plus additional features of the Github platform. GitHub offers its basic services free of charge while its more advanced features are commercially available. Some of these features are bug tracking, feature requests, and task management

To join github go to https://github.com/. Once you have created an account you can create a repository directly in Github and start working.
[insert image here]

## Creating a repository for the website
click on the + sign located in top right corner and select **"New Repository"**
