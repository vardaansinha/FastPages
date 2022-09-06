---
toc: true
layout: post
description: My attempt at changing the default remote theme for my FastPages site.
categories: [markdown,html]
title: Changing the Default Remote Theme for FastPages
---

I wanted to change the default minima theme to something else, just to see the visual effect it would have on my site.


In this first image, I changed the remote_theme section of the config.yml file to the Cayman theme, which I found online.
![]({{site.baseurl}}/images/caymanthemetestconfig.png "https://github.com/fastai/fastpages")


Then, after the changes were synced, we had the following results:
![]({{site.baseurl}}/images/caymanthemetest.png "https://github.com/fastai/fastpages")
![]({{site.baseurl}}/images/caymanthemetest2.png "https://github.com/fastai/fastpages")


As you can see, there were both positives and flaws with the design. On the positives, the color scheme is very nice, and the title font for my site looks much more appealing.

On the other hand, this theme is not adjusted with corresponding CSS, and it breaks certain components of my FastPages site. For example, my pages (tags, about me, notes, search) all disappeared, taking away from the functionality of the site. 