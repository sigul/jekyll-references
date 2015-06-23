---
layout: post
title: Adding Bigfoot js 
date: 2015-06-23 07:16:14
---

This is really simple. Just donwload the source from [bigfootjs.com](http://www.bigfootjs.com/) and then move the two files `bigfoot.js` and `bigfoot.min.js`in a folder called as you want[^1].

Move the bigfoot-default.scss file in your \_sass folder

Now open up `css/main.css` and add to the list of files to import `bigfoot-default`.

Last but not least, open up `_includes/head.html` and insert here these code:

{% highlight ruby %}
<!-- jquery-->
  <script src="//ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js"></script>
  <!-- bigfoot-->
  <script type="text/javascript" src="/bigfoot/bigfoot.min.js"></script>
  
<script type="text/javascript">
  $.bigfoot();
</script>
{% endhighlight%}

[^1]: I am calling it bigfoot, so note it because you will have to use it in the path to bigfoot files.