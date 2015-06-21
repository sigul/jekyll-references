---
layout: post
title: how to install jekyll
---
This is a post to remember me hot to install jekyll. 

It's really so simple.

1. setup a new repository on github
2. add a gh-pages branch under your master branch, and set it as the default (there's an option in the settings tab)
3. clone your gh-pages repository on your desktop
4. move readme.md file on the desktop
5. run 'jekyll new /yourlocalfolder'
6. edit _config.yml adding your repository name to baseurl (/repositoryname) and url (/repositoryname)
7. commit and sync via github app

Now your site is up and running at yourusername.github.com/repositoryname
