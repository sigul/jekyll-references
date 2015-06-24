---
layout: post
title: How to Add Social Sharing Button to Jekyll 
date: 2015-06-24 08:27:12
category: social
tag: twitter, facebook, 
---

I've discovered a tool that in a few minutes will create mobile-friendly, static sharing buttons for Facebook, Twitter, Google+ and other social media sites: [simplesharingbuttons.com](http://simplesharingbuttons.com/). It will generate buttons that will speed up your blog by not downloading unnecessary JavaScript files and keep your user's activity private. You can choose from several styles, including Font Awesome -- and it's completely free.

Here's how to add your social sharing buttons:

1. go to http://simplesharingbuttons.com/
2. design your buttons and get your codes
3. download your buttons images and copy the folder in your `/images` folder
3. add HTML code to `layouts/post.html` or in the place where you want to use them
4. modify the `src=""` of the HTML to make it point to your `/images/socialbuttons` folder [^1]. 
5. copy and paste the css code you got from Simplesharingbuttons to your main.css file, before the `@import` section.

That's it.

[^1]: Use the name of your folder instead of socialbuttons. I suggest to keep the name the folder has when you download it.
