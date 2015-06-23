---
layout: post
title: How to Create a Blog with Jekyll
date: 2015-06-21 09:03:56
---
This is a post to remember me hot to install jekyll. 

It's really so simple.

1. setup a new repository on github
2. add a gh-pages branch under your master branch, and set it as the default (there's an option in the settings tab)
3. clone your gh-pages repository on your desktop
4. move readme.md file on the desktop
5. create a local folder for your blog and run `jekyll new /yourlocalfolder`
6. edit `_config.yml adding your repository name to baseurl (`baseurl: /repositoryname`) and url (`url: /repositoryname`)
7. commit and sync via github app

Now your site is up and running at yourusername.github.com/repositoryname

To better handle it, you can manage it on your mac by running in terminal `jekyll serve --watch` (you have to be in the folder of your jekyll). Then you'll be able to view it in your browser at the url localhost:4000/yoursitename.

This is helpful when you are writing a post or creating a page and you want to get a look at how it will be rendered.

Note: If you name your repository yourname.github.io, you won't have to define a baseurl.
