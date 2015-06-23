---
layout: post
title: Adding Bigfoot js 
date: 2015-06-23 07:16:14
category: design
tag: bigfoot, footnotes
---

This is really simple. Just donwload the source from [bigfootjs.com](http://www.bigfootjs.com/) and then move the two files `bigfoot.js` and `bigfoot.min.js`in a folder called as you want[^1].

Move the bigfoot-default.scss file in your \_sass folder

Now open up `css/main.css` and add to the list of files to import `bigfoot-default`.

Last but not least, open up `_includes/head.html` and insert here these code:

{% highlight ruby %}
<!-- jquery-->
  <script src="//ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
  <!-- bigfoot-->
   <script type="text/javascript" src="{{"/bigfoot/bigfoot.min.js" | prepend: site.baseurl }}"></script>
  <script type="text/javascript">
    $.bigfoot();
  </script>
{% endhighlight%}

Note that I am using `prepand: site.baseurl` to add the name of the repository in which my blog is hosted. If you are hosting it on yourname.github.io, you won't need to use this variable, but since it is configured in `config.yml` if you let baseurl blank there this won't affect yout path to your bifgoot's files.

[^1]: I am calling it "bigfoot", so note it because you will have to use it in the path to bigfoot's files. Btw, this is a bigfoot note ;)