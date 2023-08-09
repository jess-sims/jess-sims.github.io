---
title: "How to create a Hugo Website"
date: 2023-07-08T08:06:25+06:00
description: How to create a Hugo Website
menu:
  sidebar:
    name: How to create a Hugo Website
    identifier: hugo
    weight: 50
---

Hugo is a fast, open-source static website generator with many contributors and themes available to suit various needs. It's a fantastic resource for blogs, portfolios and documentation sites and a great tool to keep web hosting costs low as Hugo sites may be hosted on github pages, netlifier and other similar services. As there are various themes available it is also relatively simple to configure a website with minimal coding and command line experience.


## Getting Started 

There are two Hugo editions to choose from, standard and extended, with extended being the recommended edition.

It is also recommends to install Git to avail of the following features: 

- Build Hugo from source
- Use the Hugo Modules feature
- Install a theme as a Git submodule
- Access commit information from a local Git repository
- Host your site with services such as CloudCannon, Cloudflare Pages, GitHub Pages, GitLab Pages, and Netlify

Please see **(link to page name)** on installing Git on Windows for further details on installing Git on Windows.  

## Install Hugo on Windows 

To install Hugo on Windows a package manager is recommended. Chocolatey is a free and open source package manager for Windows which will install the extended edition of Hugo. 

1. Via the command line run the following: 
```
choco install hugo-extended
```

2. To confirm the installation was successful:
```
hugo version
```

3. Output should be similar to:
```
> hugo version
Hugo Static Site Generator v0.78.1/extended windows/amd64 BuildDate: unknown
```


## Create a New Hugo Site

To begin creating your first Hugo site, ensure Git and Git Bash are installed on your Windows Operating System. Git and Git Bash may be installed by visiting https://git-scm.com/download/win and downloading the installer for your current Windows OS. Once the file has been downloaded, launch the installer and follow the onscreen instructions. After the installation has completed, launch Git Bash and navigate to the Desktop or another location where you would like to store your new website:

```
cd ~/Desktop/
```
</br>

Now you will execute the command to create a new Hugo site. Please note the `-f yml` option in the command below is used to create the configuration file in YAML format rather than the standard TOML format. If you woud prefer your configuration file to use TOML formatting, simlpy run the below command without the `-f yml` option: 

```
>hugo new site newHugosite -f yml
Congratulations! Your new Hugo site is created in %user%\newHugosite.

Just a few more steps and you're ready to go:

1. Download a theme into the same-named folder.
   Choose a theme from https://themes.gohugo.io/ or
   create your own with the "hugo new theme <THEMENAME>" command.
2. Perhaps you want to add some content. You can add single files
   with "hugo new <SECTIONNAME>\<FILENAME>.<FORMAT>".
3. Start the built-in live server via "hugo server".

Visit https://gohugo.io/ for quickstart guide and full documentation.
```
</br>

Via file explorer or the command line you will now observe the Hugo website folder structure and base files to be available in your newHugosite folder:

```
ls
archetypes  config.yml  content  data  layouts  public  static  themes
```

## Use a Hugo Theme 

Currently the Hugo project folder contains only the file structure and has no HTML or CSS files to create the UI of your website. Many open source themes are available to use for your website which may be used to avoid creating your website from scratch. You may view a full list of available Hugo themes here: https://themes.gohugo.io/ 

Each theme should contain it's own documentation and instructions on how to implement the theme available on the theme's preview page or an alternate source cited on the preview page. Often there will also be a running example site for preview. 

Please note you'll require a github account to clone the theme repository into your website. To create a GitHub account, visit the following link: https://github.com/

Once you have decided on a theme, navigate into the themes folder and clone the theme repository. For this example, I will be using the Hugo Profile theme: https://themes.gohugo.io/themes/hugo-profile/

Via the Hugo Profile theme preview page you will note we have been instructed to navigate into our website "themes" directory and clone the theme repository into this location:  

```
cd themes

git clone https://github.com/gurusabarish/hugo-profile.git
Cloning into 'hugo-profile'...
remote: Enumerating objects: 5348, done.
remote: Counting objects: 100% (442/442), done.
remote: Compressing objects: 100% (241/241), done.
remote: Total 5348 (delta 260), reused 311 (delta 192), pack-reused 4906
Receiving objects: 100% (5348/5348), 25.24 MiB | 3.67 MiB/s, done.
Resolving deltas: 100% (2115/2115), done.
Updating files: 100% (1687/1687), done.
```
</br>

Once the Theme has been cloned you will require to update the config.yml in the main directory of your Hugo site. For the Hugo Profile theme you will require to copy the contents from the theme YAML [file](https://github.com/gurusabarish/hugo-profile/blob/master/exampleSite/config.yaml) into your config.yml as per the documentation. Once completed, your local config.yml should appear exactly as the theme config.yaml.

## Viewing and Customizing Your Website 

Now that your website has a theme you may want to confirm that everything is configured as expected. To view a local live preview of your website, navigate to your website project directory and run the below command:
```
hugo server
```
</br>

Once completed, copy and paste the provided url output http://localhost:1313 into your browser of choice to view your current website. Hugo server will continue to run and provide live updates until it has been exited with `ctrl+c` in the terminal. As such, any changes made to the files will be reflected on screen until the task has been terminated.  

{{< img src="HugoServer.png" title="View Live Hugo Server" >}}

{{< vs 3 >}}

As every theme requires different types of customization, viewing the theme documentation for full steps is required: https://themes.gohugo.io/themes/hugo-profile/

## Conclusion

Congratulations! You have created your first hugo website using an open source theme. You may now begin to personalize your website and prepare it for a hosting service. A future article will provide further steps on launching and hosting your website.
