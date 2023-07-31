---
title: "Git and GitHub"
date: 2023-07-03T11:23:00+06:00
description: Git and GitHub
menu:
  sidebar:
    name: Git and GitHub
    identifier: git and github
    weight: 20
# hero: background-2.jpg
# math: true
---

## Introduction to Git and GitHub

Git is an extremely useful distributed version control system which allows the user to track changes to their files. Git is frequently used among developers, technical writers and other collaborative professions to manage their projects and releases. 

GitHub is a hosting service which works hand in hand with Git repositories so that collaborators may share their projects by hosting the main and current copy of the project on GitHub. From GitHub users may pull a copy of the project to their local machine, open problem reports and create branches and merge requests which may then be reviewed by the project owner(s). Git and GitHub are the cornerstone of open source computing projects allowing developers from all over the world to collaborate on projects together. 

While you do not require a GitHub account to use Git, without pushing your project to GitHub your Git progress will remain on your local machine and collaboration with others would not be so streamlined.

## Installing Git on Windows 

On Windows, Git may be installed via "Git for Windows" install located at <https://git-scm.com/download/win>.

## Creating your GitHub Account 

To create your GitHub account navigate to <https://github.com/> and click "Sign Up" in the top right hand corner. Once you have entered your email and password you'll require to confirm your email account. 

After this time you may sign into your GitHub account and navigate to your profile on the top right hand corner, settings, emails, and ensure that the below settings are enabled. 

We would suggest to take a copy of the email advised in the "Keep my email address private" setting and use this in your Git configuration setup below.

## Git Initial Configurations

Once Git has been installed there are a few tasks that are required to be completed. With the "Git for Windows" download completed earlier, this should have included the "Git Bash" program. Launch Git Bash to complete the initial configuration tasks. These tasks only need to be completed once per local system, unless you are using multiple operating systems on your machine, for example Windows Subsystem for Linux (WSL).

Firstly you'll require to confirm your identity via user name and emmail address. This information is used when you use Git commit and therefore observable in the Git log to other users. 

$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com

As it is not always advisable to have your personal email address available to anyone on the internet, it would be recommended to ensure your GitHub security options are agreeable as noted above and use the recommended GitHub email provided.

{{< img src="GitHubEmailSettings.png" height="400" title="GitHub Email Security Settings" >}}

{{< vs 3 >}}

For your name you may provide what you are comfortable with. 

## Creating your First Repro

On your local machine create a new folder named "Test" and change directory into the new directory. 

    $ cd ~/Desktop
    $ mkdir TestProject
    $ cd TestProject

To initial a new Git repository type the following command in the new directory we have created: 

    $ git init

Now add a couple new files to the directory and confirm they exist: 

    $ touch index.html
    $ touch style.css 
    $ ls 

You'll want to add all of these new files/changes to your staging area in preparation to commiting these changes to your git repository: 

    $ git add . 

To confirm which files are in the staging area or have been modified: 

    $ git status 

It's time to make your first commit to your repository. A commit moves the files and changes from the staging area into a new "save" of your files if you will. The -m flag below indicates the message to be included with the commit and it is good practice to leave relevant notes with your commits aka changes with a view that other collaborators and yourself will have a clear view of changes made over the course of a project. For example, "Created index.html file and style.css file":  

    $ git commit -m "Initial commit"

At any time you can review the Git log which displays a timeline of all commits starting with the most recent: 

    $ git log 

## Creating your First GitHub Repo

On your GitHub account profile on the top left menu you'll observe a tab called "Repositories". Click this and select "New" on the top right hand of the page. 

1. Choose a unique repository name
2. GitHub provides suggestions on unique names, if you're so inclined you can choose the name suggested for your repository 
3. (Optional) Provide a repository description 
4. Choose if the repository should be public or private. Please note the repository will require to be public if you plan to collaborate with others or use GitHub pages or another service which may require access to the repository 
5. As we're adding the files from a local folder do not create a README file at this time 
6. To learn more about ignoring files visit <https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files>
7. To learn more about chosing a license visit <https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files>
8. Create your first repository!

{{< img src="GitHubRepo.png" title="GitHub Email Security Settings" >}}

{{< vs 3 >}}

## Uploading your Repo to GitHub

As we're already made our first commit locally the following steps will require to be carried out via command line to push the local files to your newly created GitHub repo:

    git branch -M main
    git remote add origin https://github.com/jess-sims/<reponame>.git
    git push -u origin main

As this is the first time connecting to your repository, you will now be prompted to login to your GitHub account via the command line by providing your username and password.

Once this completes you should not observe your files in your GitHub repository after refreshing the page!

You should now understand the basics of creating a Git project and uploading this to a repository on your GitHub account. There are further git commands for creating new branches, merging branches, switching branches, pulling a repository from GitHub to your local machine and more, however, another article will be required to discuss these furthers. 