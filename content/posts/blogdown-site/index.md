---
categories:
- R
date: 2020-09-12
description: I spent a whole day trying to create this website using R.
displayInList: true
displayInMenu: false
draft: false
dropCap: true
resources:
- name: featuredImage
  src: headerphoto.jpg
title: Making my blog with R
---

I've been spending a bit more time on Linkedin and I see so many people posting a lot of cool stuff on their page! As an aspiring social/political/business data analyst (yes, I have a lot of interests..), I figured that I should start working on my online portfolio as well!

There are many great websites that allow you to create your own blog for free, but I wanted to feel like a smarty-pants so I decided to code my on website on R. 

I've read countless articles and watched some youtube videos on how to do this. As someone tying to get used to both R and Git, it took me a while to figure it out, but I did it anyway! So here is a complete beginner's guide to making your own blog with R!

__Summarizing the Steps__
1. Make a GitHub account and repository
2. Install blogdown and make a new site
3. Commit the code on your Git
4. Host your site

__Making a GitHub repository__
Yo, this is an important step not only for this project but also for your progress in the field. This can act as your repository for all your previous projects, so you can show them off when the time is right. Head to https://github.com/ if you still don't have one and follow all instructions to make a new account.

If you have an account just make a new Git repository like so:
![](gitrepo1.jpg)

![](gitrepo2.jpg)

Once that's done, get the URL on the tab AFTER you click confirm! You'll be needing it to link your R files to the Git!
![](gitrepo3.jpg)

ALRIGHT! Now that's done, we can head to R. Start a new R Project and click version control (File > New Project > Version Control). Fill in the form after clicking next. Input the git url from the previous step in the "Repository URL" field like so:
![](gitrepo4.jpg)

FINALLY, we can move on to the next step!

__Installing blogdown to make a new site__

There are 3 very important substeps to this step just to make sure that blogdown works:
1. Install the blogdown package: _install.packages("blogdown")_
2. Load the blogdown library: _library(blogdown)_
3. Update Hugo. Hugo is a static site generator that is connected to R blogdown. This is already built-in the blogdown package so doing this step will be a piece of cake. _blogdown::update_hugo()_

To create a new site, call: _blogdown::new_site()_
Blogdown already gives you a default template for your blog. The design isn't bad, but you might want to take a look at [Hugo Themes.](https://themes.gohugo.io/)

Now that you have a super basic canvas website and your themes, it's time to edit the content.



