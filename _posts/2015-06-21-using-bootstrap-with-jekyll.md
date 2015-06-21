---
layout: post
title: How to add Bootstrap to Jekyll
---
Adding Bootstrap to Jekyll is a little bit complicated, mainly because of the lack of istructions on the web.

I finally found this [article by Andreas Veithen](http://veithen.github.io/2015/03/26/jekyll-bootstrap.html) update at March, 2015.

In the end of the game, what you have to do to add Bootstrap to your Jekyll blog is very simple. Bootstrap uses LESS language, but there's an official port in [SASS](http://sass-lang.com/), the same language used by Jekyll. 

So, go to [getboostrap.com](http://getboostrap.com) and download the SASS port, clone it from [git repository](https://github.com/twbs/bootstrap-sass/) or download the zip file from there.

Now, you only need to follow these simple three steps:

1. Unzip the Bootstrap folder
2. Copy and paste the file _bootstrap.scss you will find in the /assets/stylesheet directory of the unzipped Bootstrap folder in your _sass folder inside your Jekyll folder
3. Copy and paste the entire /assets/styleshee/boostrap folder in your _sass folder inside your Jekyll folder
4. create a /styles/site.scss with the following code
{% highlight ruby %}
---
---
    
@import "bootstrap";
{% endhighlight %}

That's it. Look for Boostrap's variables in \_sass/bootstrap/_variables.scss.

Andreas suggest not to change this variables, because it would be more difficult to update your Bootstrap, but just override them in your styles/site.scss as follow

{% highlight ruby %}
---
---
    
$font-size-base: 17px;
$headings-font-weight: 600;
$blockquote-font-size: $font-size-base;
    
@import "bootstrap";
{% endhighlight %}
