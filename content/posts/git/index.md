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

Git is an extremely useful distributed version control system which allows the user to track changes to their files. Git is frequently used among developers, technical writers and other collaborative professions to manage their projects and releases. 

GitHub is a hosting service which works hand in hand with Git so that collaborators may share their projects by hosting the main and current copy of the project on a GitHub repository. From GitHub, users may pull a copy of the project to their local machine, open problem reports and create branches and merge requests which may then be reviewed by the project owner(s). Git and GitHub are the cornerstone of open source computing projects allowing developers from all over the world to collaborate on projects together. 

While you do not require a GitHub account to use Git, without pushing your project to GitHub your Git progress will remain on your local machine and collaboration with others would prove more difficult.

## Installing Git on Windows 

On Windows, Git may be downloaded via "Git for Windows" at <https://git-scm.com/download/win>. From the link, download the installer for your current Windows version. Once the download has completed the file will require to be opened to begin the installation process. Follow the on screen instructions to complete the installation. Please note "Git for Windows" includes the Git Bash program. 

## Creating your GitHub Account 

To create your GitHub account navigate to <https://github.com/> and click "Sign Up" in the top right hand corner. Once you have entered your email address and password you will require to confirm your email account. 

## Git Initial Configurations

Once Git has been installed there are a couple of administrative tasks that are required to be completed. The "Git for Windows" install will have included installation of the "Git Bash" program on your computer. Launch Git Bash to complete the initial configuration tasks below. Please note these tasks only require to be completed once per git installation.

Mainly, you'll require to confirm your identity via user name and email address. The information provided is logged when you make a Git commit and therefore observable in the Git log to other users. 

As it is not necessarily advisable to have your personal email address available on the internet, it would be recommended to ensure your GitHub security options are agreeable and use the recommended GitHub email provided. You may view your GitHub email address settings via navigating to your profile on the top right hand corner > settings > emails > and ensure that the below email settings are enabled. 

{{< img src="GitHubEmailSettings.png" height="400" title="GitHub Email Security Settings" >}}

{{< vs 3 >}}

To configure your git user name and email address, run the commands below with the appropriate values:

```
$ git config --global user.name "Jane Doe"
$ git config --global user.email janedoe@users.noreply.github.com
```

## Creating your First Git Project

1. Via the command line on Git Bash, navigate to your Desktop and create a new folder named "TestProject". Once the new folder has been created, change into the "TestProject" directory: 
```
$ cd ~/Desktop
$ mkdir TestProject
$ cd TestProject
```
2. To initialize Git on the project, type the following command in the new directory we have just created: 
```
$ git init
```
3. To begin, add a couple of new files to the directory and confirm that they have been created successfully: 
```
 $ touch index.html
 $ touch style.css 
 $ ls 
```
4. To add all of these new files and changes into your staging area in Git for preparation to commit: 
```
$ git add . 
```
5. To confirm which files are in the staging area or have been modified: 
```
$ git status 
```
6. It is now time to make your first git commit. A commit moves the files and changes from the staging area into a new "save" of your files with Git. The -m flag below indicates the message to be included with the commit and it is good practice to leave relevant notes with your commits with a view that yourself and other collaborators will have a clear view of changes made over the course of a project. For example, "Created index.html file and style.css file":  
```
$ git commit -m "Created index.html file and style.css file"
```
7. You can review the Git log at any time which displays a timeline of all commits starting with the most recent: 
```
$ git log 
```

## Creating your First GitHub Repo

To create your first GitHub repo, navigate to your profile on the top right hand corner. From your profile, on the top left menu you'll observe a tab called "Repositories". Click this and select "New" on the top right hand of the page. You will require to fill out the form as explained below: 

1. Choose a unique repository name
2. If you're so inclined, GitHub provides suggestions on available unique names which you may use for your repository 
3. (Optional) Provide a repository description 
4. Choose if the repository should be public or private
5. As we will be adding the files from a local folder do not create a README file at this time 
6. To learn more about ignoring files visit <https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files>
7. To learn more about chosing a license visit <https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files>
8. Create your first repository!

{{< img src="GitHubRepo.png" title="GitHub Email Security Settings" >}}

{{< vs 3 >}}

## Uploading your Files to GitHub

As you have already made your first commit locally the following steps will require to be carried out via command line to push the local files to your newly created GitHub repo:

    git branch -M main
    git remote add origin https://github.com/jess-sims/<reponame>.git
    git push -u origin main

</br>

As this is the first time connecting to your repository, you will now be prompted to authenticate your GitHub account via the command line by providing your username and password or via an alternate authentication method.

Once this completes you should now observe your files in your GitHub repository after refreshing the page!

## Conclusion

You should now understand the basics of creating a Git project and uploading this to a repository on your GitHub account. There are further git commands for creating new branches, merging branches, switching branches, pulling a repository from GitHub to your local machine and more, however, another article will be required to discuss these further. 