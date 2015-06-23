---
layout: post
title: Using Bootstrap variables in Jekyll
date: 2015-06-22 11:38:32
category: design
tag: bootstrap
---

Just use Bootstrap variables inside /_sass/_base.css.

I suppouse, but need to verify, you have to move `bootstrap` css file upper in the `main.css` @import section to avoid it's variable to be overridden by those of Jekyll.
