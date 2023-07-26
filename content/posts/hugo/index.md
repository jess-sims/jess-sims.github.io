---
title: "How to create a Hugo Website"
date: 2023-07-08T08:06:25+06:00
description: How to create a Hugo Website
menu:
  sidebar:
    name: How to create a Hugo Website
    identifier: hugo
    weight: 50
hero: boat.jpg
---

## How to create a Hugo Website

Hugo is a fast, open-source static website generator with many contributors and themes available to suit various needs. Hugo is a fantastic resource for blogs, portfolios and documentation sites. Hugo is a great tool to keep web hosting costs low as Hugo sites may be hosted on github pages, netlifier and others. As there are various themes available it is also relatively simple to configure a website with minimal coding and command line experience.

Markdown is can be used to add content to pages in Hugo. 


## Getting Started 

There are two Hugo editions to choose from, standard and extended. Hugo recommends to install the extended edition to avail of the following features: 

- Encode to the WebP format when processing images. You can decode WebP images with either edition.
- Transpile Sass to CSS using the embedded LibSass transpiler. The extended edition is not required to use the Dart Sass transpiler.

Hugo also recommends to install Git for the following features: 

- Build Hugo from source
- Use the Hugo Modules feature
- Install a theme as a Git submodule
- Access commit information from a local Git repository
- Host your site with services such as CloudCannon, Cloudflare Pages, GitHub Pages, GitLab Pages, and Netlify

## Install Hugo on Windows 

To install Hugo on Windows a package manager is recommended. Chocolatey is a free and open source package manager for Windows which will install the extended edition of Hugo:
```
choco install hugo-extended
```

To confirm the installation was successful:
```
hugo version
```

Output should be similar to:
```
> hugo version
Hugo Static Site Generator v0.78.1/extended windows/amd64 BuildDate: unknown
```


## Create a New Hugo Site

Open your command prompt, on Windows Hugo recommends to install Git Bash. 

Navigate to the folder in which to create the new project. 

```
cd Desktop 
```

Execute the Hugo new site command: 

```
>hugo new site new-hugo-website -f yml
Congratulations! Your new Hugo site is created in %user%\new-hugo-website.

Just a few more steps and you're ready to go:

1. Download a theme into the same-named folder.
   Choose a theme from https://themes.gohugo.io/ or
   create your own with the "hugo new theme <THEMENAME>" command.
2. Perhaps you want to add some content. You can add single files
   with "hugo new <SECTIONNAME>\<FILENAME>.<FORMAT>".
3. Start the built-in live server via "hugo server".

Visit https://gohugo.io/ for quickstart guide and full documentation.
```

We recommend the flag -f yml to create the configuration file in yaml as the default toml file can be finicky to edit. 

Via file explorer or command line the new Hugo website folder structure and files required for the website to function will be available. 

## Choose a Hugo Theme 

Currently the Hugo project folder contains only the file structure and has no HTML or CSS files. Many open source themes are available to customize your website if you'd like to avoid writing the entire UI yourself. View a full list of available Hugo themes here https://themes.gohugo.io/ .

Each theme should contain it's own documentation and instructions on how to implement available on the theme preview page or an alternate source cited on the preview page. Often there will also be a running example site for preview. 

You'll require a github account to clone the theme repository into your website:

```
cd themes

git clone https://github.com/gcushen/hugo-academic.git
```


## Customizing Your Website 

At your websitename directory you may run hugo to view a local live preview of your website: 
```
hugo server 
```

Copy and paste the url output http://localhost:1313 into your browser to view your current website. As changes are saved your will observe the reflections on screen. 

As themes require different customization, it would be best to review the theme documentation for full steps. 

To exit hugo server simply press ctrl+c in your terminal window. 

## Hosting your website on Github Pages

