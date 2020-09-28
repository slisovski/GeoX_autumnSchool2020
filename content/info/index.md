---
aliases: [arm]
title: "Website contributions"
summary: ""
abstract: ""
date: "2020-09-24T00:00:00Z"
image:
  caption:
  focal_point: Smart
categories:
tags:
---

This website is made with [github](https://github.com/slisovski/GeoX_autumnSchool2020), the [blogdown](https://bookdown.org/yihui/blogdown/) R package, and the Academic theme for [Hugo](https://themes.gohugo.io/academic/). The infrastructure allows you to directly contribute to the website. If you are familiar with RStudio, R Markdwon and GitHub, you can start immediately. Other options via text editor and git are possible too. However, a short introduction migth help to get you started:

## Initial setup

### Cloning the homepage repo

- Make a github account [here](https://github.com/).
- Ask Simeon ([simeon.lisovski@gmail.com](mailto:simeon.lisovski@gmail.com)) to be added as a collaborator to the repo.
- Open your terminal (or R studio) and navigate to a directory where you'd like to clone the repository.
- Run this command in your terminal (or in git bash or while you create a blockdown project in RStudio): 

```
git clone --recursive -j8 https://github.com/slisovski/GeoX_autumnSchool2020.git
```

- Check that you're on the master branch both in the root directory, as well as in the subfolder public.
- In the root directory, run the following commands:

```
git branch 
cd public
git branch 
cd ../themes/academic
git branch
```
You should be on the branch `master` for all three of them. If not, then type `git checkout master` to change the branch (in each of the three directories).

### Installing `hugo` (not nessesary if you work with RStudio)

- First, install `homebrew` following the instructions [here](https://brew.sh/).
- The current version of the homepage works with hugo version 0.55.5. To install this particular version, run the following commands (see [this post](https://www.fernandomc.com/posts/brew-install-legacy-hugo-site-generator/) for more info).

```
brew unlink hugo
brew install https://raw.githubusercontent.com/Homebrew/homebrew-core/2d7e602ad4c26d1d509e5f6c17fd5911323788a3/Formula/hugo.rb
```

## The research project folder

```
...
├── content
│   ├── home
│   ├── info
│   ├── project
│   └── projects
...
```
- `content`: contains markdown files used to render the page 
	+ `home`: all widgets displayed on the first page 
	+ `info`: this site 
	+ `project`: the project folders
	+ `projects`: widget for project site
	
### Change your project site

- In the project folder you will find the index.md file.
- Make changes (include text, images etc.)

### Commit changes and push to repository.