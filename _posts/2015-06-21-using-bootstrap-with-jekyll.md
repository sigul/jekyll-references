---
layout: post
date:   2015-06-21 13:03:56
title: How to add Bootstrap to Jekyll
category: design
---
Adding Bootstrap to Jekyll is a little bit complicated, mainly because of the lack of istructions on the web.

I finally found this [article by Andreas Veithen](http://veithen.github.io/2015/03/26/jekyll-bootstrap.html) update at March, 2015. I used that, but I did a few changes to simplify it (actually, I didn't understand the necessity to add a different file from main.css to import bootstrap.css).

In the end of the game, what you have to do to add Bootstrap to your Jekyll blog is very simple. Bootstrap uses LESS language, but there's an official port in [SASS](http://sass-lang.com/), the same language used by Jekyll. 

So, go to [getboostrap.com](http://getboostrap.com) and download the SASS port, clone it from [git repository](https://github.com/twbs/bootstrap-sass/) or download the zip file from there.

Now, you only need to follow these simple three steps:

1. Unzip the Bootstrap folder
2. Copy and paste the file `_bootstrap.scss` you will find in the `/assets/stylesheet/` directory of the unzipped Bootstrap folder in your `_sass folder inside your Jekyll folder
3. Copy and paste the entire `/assets/stylesheet/boostrap` folder in your `_sass` folder inside your Jekyll folder
4. add `bootstrap` to main.css file in the css folder under line starting with `@import`.

That's it. Look for Boostrap's variables in `_sass/bootstrap/_variables.scss`and use them in your blog.

Andreas suggest not to change this variables, because it would be more difficult to update your Bootstrap. You can override them in your main.css as follow, in the `// Our variables` section.